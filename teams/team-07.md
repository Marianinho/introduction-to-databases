CREATE DATABASE IF NOT EXISTS SigaaSalas;
USE SigaaSalas;


CREATE TABLE SigaaID (
    IdSala INT AUTO_INCREMENT PRIMARY KEY NOT NULL
);


CREATE TABLE SigaaTipoSala (
    TipoSalaID INT AUTO_INCREMENT PRIMARY KEY NOT NULL,
    TipoSala VARCHAR(25)
);

INSERT INTO SigaaTipoSala (TipoSala)
VALUES
('Banheiro'),
('Sala de estudo'),
('Sala de computadores'),
('Sala de Reunião'),
('Sala da limpeza'),
('Sala RH');

CREATE TABLE SigaaHorario (
    HorarioDeUso INT AUTO_INCREMENT PRIMARY KEY,
    
    FOREIGN KEY (TipoSalaID)
        REFERENCES SigaaTipoSala(TipoSalaID)
);


CREATE TABLE SigaaMateriais (
    MaterialID INT AUTO_INCREMENT PRIMARY KEY,
    IdSala INT,
    Materiais VARCHAR(25),
    QtdMateriais INT NOT NULL,
    MatPrincipal BOOLEAN,
	
    FOREIGN KEY (IdSala)
        REFERENCES SigaaID(IdSala)
);

INSERT INTO SigaaMateriais (Materiais)
VALUES
('Cadeira'),
('Mesas'),
('Projetores'),
('Canetão'),
('Computadores');

CREATE TABLE SigaaSalas (
    IdSala INT PRIMARY KEY AUTO_INCREMENT,

    TipoSalaID INT,
    HorarioDeUso INT,
    MateriaisID INT,

    FOREIGN KEY (TipoSalaID)
        REFERENCES SigaaTipoSala(TipoSalaID),

    FOREIGN KEY (HorarioDeUso)
        REFERENCES SigaaHorario(HorarioDeUso),

	FOREIGN KEY (MateriaisID)
		REFERENCES SigaaMateriais(MaterialID)
);

SELECT
    s.IdSala,
    ts.TipoSala AS TipoSalas,
    h.HorarioDeUso,
    m.Materiais AS MatPrincipal,
    m.QtdMateriais

FROM SigaaSalas s

JOIN SigaaTipoSala ts
    ON s.TipoSalaID = ts.TipoSalaID

JOIN SigaaHorario h
    ON s.HorarioDeUso = h.HorarioDeUso

JOIN SigaaMateriais m
    ON s.MateriaisID = m.MaterialID

WHERE m.MatPrincipal = TRUE;
