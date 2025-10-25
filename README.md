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


## 🚀 Carregamento de Dados

O notebook solicita o upload do arquivo de dados de entrada (`ClassTT_01_tiny.txt` ou similar) através da função `files.upload()`.

1.  Abra o arquivo `IA_P01_G03.ipynb`.
2.  Execute a célula de instalação.
3.  Quando solicitado, carregue o arquivo de dados.
4.  Execute as células subsequentes para carregar os dados e construir o modelo.

## 🛠️ Estrutura e Dados

### Domínio do Problema

Os domínios de tempo e espaço para a alocação de horários são definidos pelas seguintes constantes:

* **Dias (`DAYS`):** `['Mon', 'Tue', 'Wed', 'Thu', 'Fri']`
* **Blocos de Tempo (`BLOCKS`):** 1 a 20 (4 blocos por dia, 5 dias por semana)
* **Salas (`ROOMS`):** `['R1', 'R2', 'R3', 'R4', 'Lab01', 'Online']`

### Estruturas de Dados Carregadas

A função `load_timetable_data` parseia os dados de entrada (`.txt`) e os armazena nas seguintes estruturas (baseadas nos *headers* do arquivo):

| Variável | Header no Arquivo | Descrição |
| :--- | :--- | :--- |
| **`CLASS_COURSES`** | `#cc` | Disciplinas atribuídas a cada Turma. |
| **`TEACHER_COURSES`** | `#dsd` | Disciplinas lecionadas por cada Professor. |
| **`TEACHER_UNAVAILABLE_SLOTS`** | `#tr` | Slots de tempo em que um Professor está indisponível. |
| **`COURSE_ROOM_RESTRICTIONS`** | `#rr` | Restrições de sala específicas para uma Disciplina (ex: requer Lab01). |
| **`ONLINE_LESSONS`** | `#oc` | Disciplinas marcadas como aulas online. |

## 🧑‍💻 Autor

* **Grupo:** G03
* **Contexto:** IA25_P01_G03
* **Trabalho:** TRAB 1 cadeira de AI
