# 📅 IA25_P01_G03: Resolução do Problema de Horários (Timetable Scheduling)

## 🌟 Descrição do Projeto

Este projeto é o **Trabalho 1 (TRAB 1)** para a cadeira de **Inteligência Artificial (AI)**. O objetivo é resolver o problema de alocação de horários (Timetable Scheduling) utilizando o paradigma de **Programação por Restrições (Constraint Satisfaction Problem - CSP)**.

O notebook `IA_P01_G03.ipynb` implementa um modelo de CSP que atribui horários (`BLOCKS`) e salas (`ROOMS`) a aulas, respeitando um conjunto de restrições complexas extraídas de um arquivo de dados.

## ⚙️ Tecnologias Utilizadas

O projeto é desenvolvido em Python e utiliza a seguinte biblioteca:

| Tecnologia | Descrição |
| :--- | :--- |
| **Python** | Linguagem de programação principal. |
| **`python-constraint`** | Biblioteca utilizada para modelar e resolver o problema de Programação por Restrições (CSP). |
| **Jupyter/Colab** | Ambiente de desenvolvimento e execução do código. |

## 🚀 Como Executar o Projeto

Para executar o projeto, siga os passos abaixo no ambiente do Google Colab ou em um ambiente Jupyter local:

### 1. Instalação de Dependências

A primeira célula do notebook instala automaticamente a biblioteca necessária:

```bash
!pip install python-constraint
