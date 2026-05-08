# 📊 Credit Score Prediction (Previsão de Score de Crédito)

Este projeto aplica técnicas de Machine Learning para automatizar a análise e classificação de risco de crédito de clientes bancários. A partir de um histórico financeiro e comportamental, o modelo prevê se o *score* de crédito do cliente será classificado como **Poor (Ruim)**, **Standard (Regular)** ou **Good (Bom)**.

## 🎯 Objetivo
Substituir a análise manual de crédito por um sistema preditivo automatizado, garantindo maior agilidade, precisão e padronização na tomada de decisão.

## 🛠️ Tecnologias Utilizadas
- **Linguagem:** Python
- **Manipulação de Dados (ETL):** `pandas`
- **Machine Learning:** `scikit-learn` (Random Forest, K-Nearest Neighbors, Label Encoding)
- **Ambiente:** Jupyter Notebook

## ⚙️ Arquitetura e Fluxo do Projeto
1. **Extração:** Leitura da base de dados de clientes (`clientes.csv`).
2. **Pré-processamento:** Tratamento de valores nulos e codificação de variáveis categóricas (texto para números) utilizando `LabelEncoder`.
3. **Divisão dos Dados:** Separação das bases de treino (70%) e teste (30%) utilizando o `train_test_split`.
4. **Modelagem:** Treinamento de dois algoritmos de classificação:
   - *Random Forest Classifier*
   - *K-Neighbors Classifier (KNN)*
5. **Avaliação:** Comparação de acurácia, onde o modelo **Random Forest** apresentou o melhor desempenho (~83%).
6. **Previsão:** Aplicação do modelo vencedor em uma nova base de dados (`novos_clientes.csv`) para gerar as classificações finais.

## 🚀 Como Executar
1. Clone este repositório:
   ```bash
   git clone 
   ```
2. Instale as dependências necessárias:
   ```bash
    pip install pandas scikit-learn jupyter
   ```
3. Abra o arquivo `main.ipynb` e execute as células sequencialmente.

## 📈 Próximos Passos
* Refinar a engenharia de recursos (Feature Engineering).
* Exportar o modelo treinado para consumo em uma API.
* Construir um dashboard de acompanhamento dos perfis de crédito.
