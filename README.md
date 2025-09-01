# desafio-ciencia-de-dados-imdb

## Objetivo do projeto
Analisar uma base de dados de filmes do IMDb para entender quais fatores influenciam seu sucesso, como faturamento e notas do público, além de criar um modelo para prever a nota do filme de exemplo.

---

## 🛠️ Tecnologias e Bibliotecas

- **Linguagem:** Python 3  
- **Pandas:** Manipulação e análise de dados  
- **NumPy:** Operações matemáticas e arrays  
- **Seaborn & Matplotlib:** Visualização de dados  
- **Scikit-Learn:** Criação e avaliação de modelos de Machine Learning  
- **Joblib:** Salvamento e carregamento de modelos

---

## 📂 Estrutura do Projeto

```text
├── LH CD Marcelo Augusto Mouro Junior.ipynb   # Notebook com o código e análises
├── README.md                                 # Documentação do projeto
├── Modelo de Avaliação IMDB.pkl              # Modelo treinado salvo
└── requirements.txt                          # Dependências do projeto
```
---

## 📊 Resultados e Respostas

1. **Análise Exploratória dos Dados (EDA)**  
   Foram analisadas as principais características do dataset, identificando correlações entre variáveis, padrões de faturamento e notas.  
   Destaque para:
   - Relação entre **número de votos** e **faturamento**: filmes com maior engajamento tendem a faturar mais.
   - Distribuição de notas do IMDb concentrada entre 6 e 8.
   - Insights de palavras-chave na sinopse (Overview) para identificação de gênero.

---

2. **Respostas às Perguntas:**

**a) Qual filme você recomendaria para uma pessoa que você não conhece?**  
🎬 *The Shawshank Redemption* (Nota IMDb: **9.3**)

---

**b) Quais são os principais fatores relacionados com alta expectativa de faturamento?**  
📈 O **número de votos (No_of_Votes)** é o fator com maior correlação positiva com o faturamento.  
Filmes com grande engajamento do público tendem a gerar maior receita.

---

**c) Quais insights podem ser tirados da coluna Overview?**  
📖 A sinopse pode ser usada para:
- Extrair palavras-chave que indiquem o gênero do filme.  
  Exemplos:
  - Termos como *"war"*, *"battle"* e *"soldier"* → Filmes de guerra  
  - Termos como *"love"*, *"romance"* e *"relationship"* → Filmes românticos  

---

3. **Previsão da Nota IMDb**  
- Tipo de problema: **Regressão**  
- Variáveis escolhidas: `Meta_score`, `No_of_Votes`, `Runtime`  
- Modelo: **Regressão Linear** (pela simplicidade e boa interpretabilidade)  
- Métricas de avaliação:
  - **MAE (Erro Absoluto Médio)** ≈ 0.19  
  - **RMSE (Raiz do Erro Quadrático Médio)** ≈ 0.23  
📊 Resultado: O modelo apresentou **boa precisão** para prever a nota do IMDb.

---

4. **Nota prevista para o filme de exemplo:**  
🎯 **8.86**

---

## ▶️ Como Executar o Projeto

1. **Clonar o repositório:**
   ```bash
   git clone https://github.com/marcelomourojr/desafio-ciencia-de-dados-imdb.git
   cd desafio-ciencia-de-dados-imdb

2.	Instalar dependências:
   	```bash
	pip install -r requirements.txt

3.	Abrir o Notebook:

	•	No Google Colab: <br> 
Fazer upload do arquivo notebook.ipynb e do arquivo Desafio Indicium IMDB.csv antes de rodar.<br>

	•	Localmente (Jupyter Notebook/Lab):<br> 
Rodar o notebook diretamente, pois o CSV já estará na pasta do projeto.
