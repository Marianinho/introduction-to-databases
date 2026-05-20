# Introduction to Databases

## Projeto Colaborativo de Banco de Dados

Este repositório contém o projeto colaborativo desenvolvido pelos alunos da disciplina de Banco de Dados.

O principal objetivo é simular um fluxo real de desenvolvimento de software utilizando:

* MySQL Workbench
* Banco de Dados Relacional
* Colaboração com GitHub
* Forks
* Commits
* Pull Requests

---

# Objetivo do Projeto

Desenvolver um sistema de banco de dados relacional completo aplicando os conceitos de:

* Chave Primária (PK)
* Chave Estrangeira (FK)
* Relacionamentos entre tabelas
* Consultas SQL
* Operações JOIN
* Fluxo colaborativo de desenvolvimento

---

# Tema Principal do Sistema

Toda a turma irá desenvolver colaborativamente um único sistema de banco de dados.

Cada equipe será responsável por um módulo específico do sistema.

---

# Responsabilidades das Equipes

## Team 01 — Módulo de Alunos

Responsável por:

* tabela de alunos
* registros de alunos
* consultas básicas de alunos

---

## Team 02 — Módulo de Cursos

Responsável por:

* tabela de cursos
* registros de cursos
* consultas de cursos

---

## Team 03 — Módulo de Professores

Responsável por:

* tabela de professores
* registros de professores
* consultas de professores

---

## Team 04 — Módulo de Disciplinas

Responsável por:

* tabela de disciplinas
* registros de disciplinas
* consultas de disciplinas

---

## Team 05 — Módulo de Matrículas

Responsável por:

* tabela de matrículas
* relacionamentos entre alunos e disciplinas
* consultas de matrícula

---

## Team 06 — Módulo de Notas

Responsável por:

* tabela de notas
* registros de notas
* consultas de notas

---

## Team 07 — Módulo de Salas

Responsável por:

* tabela de salas
* registros de salas
* consultas de salas

---

## Team 08 — Módulo de Departamentos

Responsável por:

* tabela de departamentos
* registros de departamentos
* consultas de departamentos

---

## Team 09 — Módulo de Frequência

Responsável por:

* tabela de frequência
* registros de frequência
* consultas de frequência

---

## Team 10 — Módulo da Biblioteca

Responsável por:

* tabela de livros
* tabela de autores
* consultas da biblioteca

---

## Team 11 — Módulo Financeiro

Responsável por:

* tabela de pagamentos
* registros financeiros
* consultas de pagamentos

---

## Team 12 — Módulo de Horários

Responsável por:

* tabela de horários
* consultas de horários de aula

---

## Team 13 — Consultas JOIN

Responsável por:

* operações JOIN avançadas
* consultas integradas
* consultas relacionais

---

## Team 14 — Documentação do Banco de Dados

Responsável por:

* diagrama ER
* modelo relacional
* organização da documentação

---

## Team 15 — Validação de Dados

Responsável por:

* revisão dos INSERTs
* validação dos relacionamentos
* testes dos scripts SQL

---

## Team 16 — Integração Final

Responsável por:

* organização final dos scripts SQL
* integração dos módulos
* preparação da estrutura final do projeto

---

# Estrutura do Repositório

```bash
/docs
/sql
/teams
```

---

# Descrição das Pastas

## /docs

Contém:

* Diagrama ER
* Modelo Relacional
* Documentação do Sistema

---

## /sql

Contém:

* CREATE DATABASE
* CREATE TABLE
* INSERT INTO
* consultas SELECT
* consultas JOIN

Esses arquivos serão organizados e integrados pelo professor ao longo do projeto.

---

## /teams

Contém:

* arquivos individuais de cada equipe;
* progresso do desenvolvimento;
* scripts SQL;
* consultas;
* documentação;
* screenshots.

Cada equipe deverá trabalhar SOMENTE no seu arquivo:

```bash
team-01.md
team-02.md
team-03.md
...
team-16.md
```

---

# Como Cada Equipe Deve Preencher o Arquivo

Cada equipe deverá adicionar dentro do seu arquivo:

* nome dos integrantes;
* descrição do módulo;
* CREATE TABLE;
* INSERT INTO;
* consultas SELECT;
* consultas JOIN;
* screenshots do MySQL Workbench;
* observações do projeto.

---

# Modelo Esperado Dentro do team-XX.md

````markdown
# Team XX — Nome do Módulo

## Integrantes

- Nome 1
- Nome 2

---

# Descrição

Descrição breve do módulo.

---

# CREATE TABLE

```sql
CREATE TABLE example (
    id INT PRIMARY KEY
);
```

---

# INSERT INTO

```sql
INSERT INTO example VALUES (1);
```

---

# CONSULTAS SQL

## SELECT *

```sql
SELECT * FROM example;
```

---

## SELECT COM WHERE

```sql
SELECT * FROM example
WHERE id = 1;
```

---

## SELECT COM ORDER BY

```sql
SELECT * FROM example
ORDER BY id;
```

---

# JOIN

```sql
SELECT *
FROM example;
```

---

# Screenshots

Inserir screenshots do MySQL Workbench abaixo.
````

---

# Fluxo de Trabalho no GitHub

Cada equipe DEVE seguir o fluxo abaixo:

---

## Passo 1 — Fazer Fork do Repositório

Clique no botão "Fork" no GitHub para criar uma cópia do repositório em sua conta.

---

## Passo 2 — Abrir a Pasta /teams

Após realizar o Fork:

* abra a pasta `/teams`;
* localize o arquivo correspondente à sua equipe.

Exemplo:

```bash
team-05.md
```

---

## Passo 3 — Editar o Arquivo da Equipe

Clique no ícone de lápis (✏️) para editar o arquivo diretamente no GitHub.

Cada equipe deve modificar SOMENTE o seu arquivo.

---

## Passo 4 — Inserir o Conteúdo do Projeto

Adicionar:

* SQL;
* INSERTs;
* consultas;
* JOINs;
* screenshots;
* documentação.

Tudo deve ficar dentro do arquivo `team-XX.md`.

---

## Passo 5 — Fazer Commit das Alterações

Após finalizar as alterações:

* clique em "Commit changes";
* escreva uma mensagem clara para o commit.

Exemplo:

```bash
Team 05 - atualização do módulo de matrículas
```

---

## Passo 6 — Criar Nova Branch

Ao realizar o commit:

NÃO utilizar:

```text
Commit directly to the main branch
```

Selecionar SEMPRE:

```text
Create a new branch for this commit and start a pull request
```

Isso garante:

* organização do projeto;
* validação automática;
* revisão do professor;
* funcionamento correto do Pull Request.

---

## Passo 7 — Abrir Pull Request

Após criar a nova branch:

* clique em "Propose changes";
* revise as alterações;
* clique em "Create Pull Request".

O professor irá revisar:

* organização;
* estrutura;
* SQL;
* documentação;
* funcionamento do projeto.

Somente Pull Requests aprovados serão integrados ao repositório principal.

---

# Requisitos de Entrega

Cada equipe deverá entregar:

* scripts SQL;
* comandos INSERT;
* consultas SELECT;
* consultas JOIN;
* screenshots;
* documentação do módulo.

---

# Regras Importantes

* NÃO modificar arquivos de outras equipes.
* Trabalhar apenas no arquivo correspondente à sua equipe.
* NÃO realizar commits diretamente na branch `main`.
* Utilizar mensagens de commit claras.
* Manter o repositório organizado.
* Todos os scripts SQL devem funcionar corretamente.
* Pull Requests com erros poderão ser rejeitados.

---

# Tecnologias Utilizadas

* MySQL Workbench
* SQL
* GitHub

---

# Repositório Oficial

https://github.com/brenofeliix/introduction-to-databases
