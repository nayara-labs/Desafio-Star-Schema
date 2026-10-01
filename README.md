# ⭐ Desafio de Modelagem Dimensional - Star Schema

## 📌 Objetivo

Desenvolver um modelo dimensional em formato Star Schema com foco na análise de dados relacionados aos professores, conforme proposto na atividade.

O objetivo foi transformar o modelo relacional disponibilizado com o Power BI em uma estrutura de um esquema dimensional – star schema voltada para análise de dados, identificando a tabela fato e as tabelas dimensão necessárias para suportar consultas analíticas. 
Porém o modelo disponibilizado com o Power BI foi o "finalcial_sample" e o pedido era o de "universidade". Portanto criei do zero.

---

## 🏗️ Estrutura Desenvolvida

Foi criada a tabela fato **F_Professor**, contendo as chaves que relacionam as principais informações do processo analisado.

Também foram criadas as seguintes tabelas dimensão:

- D_Professor
- D_Departamento
- D_Curso
- D_Disciplina
- D_Data

A dimensão de datas foi criada conforme solicitado na atividade, permitindo análises temporais por ano e semestre.

---

## 🌟 Modelo Star Schema

A tabela fato foi posicionada no centro do modelo e conectada às dimensões através de relacionamentos do tipo um-para-muitos, facilitando consultas analíticas e futuras visualizações em ferramentas de Business Intelligence.

### Tabela Fato

**F_Professor**

Campos utilizados:

- idProfessor
- idDepartamento
- idCurso
- idDisciplina
- idData

### Tabelas Dimensão

**D_Professor**
- idProfessor

**D_Departamento**
- idDepartamento
- Departamento

**D_Curso**
- idCurso
- Curso

**D_Disciplina**
- idDisciplina
- Disciplina

**D_Data**
- idData
- Ano
- Semestre

---

## 🔍 Justificativa da Modelagem

O professor foi definido como objeto principal de análise, conforme solicitado pelo desafio.

A tabela fato concentra os relacionamentos entre professor, departamento, curso, disciplina e período de oferta, enquanto as dimensões armazenam os atributos descritivos necessários para as análises.

---

## 📅 Dimensão Data

Como o modelo relacional fornecido não possuía informações temporais, foi criada uma dimensão de datas contendo atributos de Ano e Semestre, permitindo a realização de análises históricas e evolução temporal das ofertas acadêmicas.

---


---

## 👩‍💻 Autora

Projeto desenvolvido por **Nayara** como parte da formação em Dados da DIO.
