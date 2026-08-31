# SPRINT 1/5 — Planejamento Inicial do Módulo

**Disciplina:** Laboratório de Banco de Dados  
**Data:** 31/08/2026  
**Equipe:** Team 01  
**Módulo:** Alunos  

---

## Objetivo da Sprint 1/5

Nesta primeira etapa, a equipe deverá **planejar o módulo sob sua responsabilidade antes de iniciar a implementação em SQL**.

O objetivo de hoje é definir claramente:

- quem são os integrantes da equipe;
- qual é a responsabilidade do módulo;
- quais dados deverão ser armazenados;
- quais atributos farão parte da tabela principal;
- qual será a chave primária;
- quais restrições de integridade serão necessárias;
- quais outros módulos poderão se relacionar com este módulo.

> **Importante:** nesta Sprint ainda não é necessário implementar `CREATE TABLE`, `INSERT`, `UPDATE`, `DELETE` ou consultas SQL. Esses conteúdos serão desenvolvidos nas próximas aulas.

---

## 1. Integrantes

Preencha com os integrantes da equipe.

- Nome completo:
- Nome completo:
- Nome completo:
- Nome completo:

---

## 2. Descrição do módulo

Escreva uma breve descrição explicando o papel do **Módulo de Alunos** dentro do sistema.

A descrição deve responder:

1. O que este módulo representa?
2. Quais informações principais serão armazenadas?
3. Para que essas informações serão utilizadas?
4. Com quais outros módulos ele poderá se relacionar?

### Exemplo de nível esperado

> O Módulo de Alunos será responsável por armazenar e organizar os dados acadêmicos básicos dos estudantes cadastrados no sistema. Esses dados poderão posteriormente ser utilizados por outros módulos, como matrículas, notas, frequência e biblioteca.

**Não copie o exemplo literalmente. Produza a descrição da própria equipe.**

### Descrição da equipe

> Escreva aqui.

---

## 3. Planejamento da tabela principal

A equipe deverá definir os atributos iniciais da tabela responsável por representar os alunos.

Preencha a tabela abaixo.

| Atributo | Tipo de dado previsto | Obrigatório? | Restrição prevista | Justificativa |
|---|---|---|---|---|
| `id_aluno` | `INT` | Sim | `PRIMARY KEY` | Identificador único do aluno |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |
|  |  |  |  |  |

A equipe deverá propor **pelo menos 5 atributos além do identificador principal**.

Alguns exemplos de atributos que podem ser considerados:

- nome;
- matrícula;
- e-mail;
- data de nascimento;
- data de ingresso;
- situação acadêmica.

A equipe não é obrigada a utilizar exatamente esses atributos.

---

## 4. Chave primária

Informe qual atributo será utilizado como chave primária da tabela.

**Atributo escolhido:**

`________________________________________`

### Justificativa

Explique por que esse atributo é adequado para identificar cada registro de forma única.

> Escreva aqui.

---

## 5. Restrições de integridade

Identifique quais restrições poderão ser necessárias.

| Atributo | Restrição prevista | Justificativa |
|---|---|---|
|  | `NOT NULL`, `UNIQUE`, etc. |  |
|  |  |  |
|  |  |  |
|  |  |  |

Durante a discussão, considere perguntas como:

- dois alunos podem possuir a mesma matrícula?
- dois alunos podem possuir o mesmo e-mail?
- o nome de um aluno pode ficar vazio?
- quais informações devem ser obrigatórias?
- quais dados precisam ser únicos?

---

## 6. Relacionamentos com outros módulos

Liste os módulos que poderão utilizar ou se relacionar com os dados de alunos.

| Módulo relacionado | Como poderá se relacionar com Alunos? |
|---|---|
| Matrículas | |
| Notas | |
| Frequência | |
| Biblioteca | |
| Outro, se necessário | |

> Nesta Sprint, não é necessário implementar `FOREIGN KEY`. O objetivo é apenas identificar possíveis relacionamentos.

---

## 7. Regras de negócio identificadas

Registre pelo menos **3 regras de negócio** que a equipe considera importantes para o módulo.

Exemplos de perguntas que podem ajudar:

- todo aluno deve possuir matrícula?
- uma matrícula pode se repetir?
- um aluno pode existir sem e-mail?
- o sistema deverá registrar a situação acadêmica do aluno?

### Regras da equipe

1. 
2. 
3. 

---

## 8. Dúvidas ou decisões pendentes

Registre aqui pontos que ainda precisam ser discutidos com o professor ou com outras equipes.

- 
- 
- 

Caso não existam dúvidas, escreva:

> Nenhuma dúvida pendente nesta Sprint.

---

## 9. Checklist da Sprint 1/5

Antes de finalizar a atividade de hoje, verifique se a equipe completou:

- [ ] identificação dos integrantes;
- [ ] descrição do módulo;
- [ ] definição da tabela principal;
- [ ] pelo menos 5 atributos além da chave primária;
- [ ] escolha e justificativa da chave primária;
- [ ] identificação das principais restrições;
- [ ] identificação dos relacionamentos com outros módulos;
- [ ] definição de pelo menos 3 regras de negócio;
- [ ] registro de dúvidas ou decisões pendentes;
- [ ] revisão do arquivo antes do commit.

---

## 10. Entrega da Sprint 1/5

O arquivo desta etapa deverá ser salvo com o nome:

```text
SPRINT1-5.md
```

e permanecer dentro da pasta da equipe:

```text
teams/Teams-UNEMAT/team-01/SPRINT1-5.md
```

A equipe deverá realizar um commit ao final da atividade.

### Sugestão de mensagem de commit

```text
Team 01 - conclui Sprint 1 de 5
```

---

## Próxima etapa

Na **Sprint 2/5**, a equipe utilizará o planejamento produzido hoje para implementar a estrutura do banco de dados utilizando comandos DDL, especialmente:

- `CREATE TABLE`;
- tipos de dados;
- `PRIMARY KEY`;
- `FOREIGN KEY`;
- `NOT NULL`;
- `UNIQUE`;
- `DEFAULT`;
- `ALTER TABLE`, quando necessário.

> **Não antecipe a Sprint 2/5 neste arquivo.** A atividade de hoje será avaliada exclusivamente pelo planejamento registrado na Sprint 1/5.
