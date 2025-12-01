# 🎓 Previsão de Desempenho Acadêmico com Machine Learning

Este projeto foi desenvolvido como parte da avaliação da disciplina de **Inteligência Computacional**. O objetivo é aplicar algoritmos de Machine Learning para prever a nota final de alunos com base em dados socioeconômicos e histórico escolar.

## 📌 Sobre o Problema
O desempenho acadêmico é influenciado por diversos fatores, desde o tempo de estudo até o consumo de álcool e a estrutura familiar. Utilizando dados históricos, construímos modelos preditivos para estimar a nota final (`G3`) de estudantes de matemática.

**Tipo de Problema:** Regressão (Aprendizado Supervisionado).

## 📊 Base de Dados
Utilizamos o **Student Performance Data Set** do repositório da UCI Machine Learning Repository.
- **Fonte:** [UCI Archive](https://archive.ics.uci.edu/dataset/320/student+performance)
- **Tamanho:** 395 instâncias (alunos).
- **Entradas:** 33 atributos (escola, idade, tamanho da família, tempo de estudo, faltas, etc.).

## 🛠 Tecnologias Utilizadas
- **Linguagem:** Python
- **Ambiente:** Google Colab
- **Bibliotecas:** Pandas, Scikit-learn, Matplotlib, Seaborn.

## 🧠 Modelos Avaliados
Testamos três algoritmos com as seguintes métricas de desempenho no conjunto de teste:

| Modelo | MAE (Erro Médio Absoluto) | MSE (Erro Quadrático) | R² (Precisão) |
| :--- | :---: | :---: | :---: |
| Regressão Linear | 1.65 | 5.66 | 0.72 |
| **Random Forest (Campeão)** 🏆 | **1.16** | **3.80** | **0.81** |
| Rede Neural (MLP) | 1.45 | 5.61 | 0.72 |

## 📈 Conclusões
O modelo **Random Forest** obteve o melhor desempenho, explicando cerca de **81%** da variação das notas.
A análise de importância de atributos revelou que as notas anteriores (`G2` e `G1`) são os maiores preditores, seguidas pelo número de faltas (`absences`).

## 👥 Autores
- Karolinny Oliveira
- Jonas Fernandes
