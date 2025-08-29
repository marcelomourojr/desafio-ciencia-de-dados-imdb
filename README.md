# desafio-ciencia-de-dados-imdb

# 🎬 Desafio Ciência de Dados - Previsão de Nota IMDb

Este projeto foi desenvolvido como parte do processo seletivo para **Trainee em Ciência de Dados**.  
O objetivo foi analisar um conjunto de dados de filmes e criar um modelo simples capaz de **prever a nota IMDb** de um filme a partir de informações como `Meta_score`, `No_of_Votes` e `Runtime`.

---

## 🚀 Objetivos do Projeto
- Analisar dados de filmes com **Análise Exploratória de Dados (EDA)**.
- Identificar fatores relacionados ao **faturamento (Gross)**.
- Explorar a coluna `Overview` e entender como o texto pode ajudar na classificação de gênero.
- Criar um **modelo preditivo** para prever a nota IMDb de filmes.
- Testar o modelo com o exemplo do filme *The Shawshank Redemption*.
- Salvar o modelo treinado no formato `.pkl`.

---

## 🛠️ Tecnologias e Bibliotecas
- [Python 3](https://www.python.org/)
- [Pandas](https://pandas.pydata.org/)
- [NumPy](https://numpy.org/)
- [Seaborn](https://seaborn.pydata.org/)
- [Matplotlib](https://matplotlib.org/)
- [Scikit-Learn](https://scikit-learn.org/stable/)
- [Joblib](https://joblib.readthedocs.io/)

---

## 📊 Principais Resultados
- A **nota IMDb** pôde ser prevista com boa precisão (MAE ≈ 0.19).  
- O **número de votos** foi o fator mais relacionado ao faturamento.  
- A coluna `Overview` tem potencial para classificar filmes usando **NLP**.  
- A previsão para *The Shawshank Redemption* foi **8.86** (próxima da nota real de 9.3).  

---

## 📁 Estrutura do Projeto
├── Desafio Indicium IMDB.csv   # Base de dados
├── imdb_rating_model.pkl       # Modelo salvo
├── notebook.ipynb              # Notebook com o código
├── requirements.txt            # Dependências do projeto
└── README.md                   # Documentação do projeto

---

## ▶️ Como Executar o Projeto
1 -  **Clonar o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/desafio-imdb.git
   cd desafio-imdb

2 - **Instalar dependências:**
   pip install -r requirements.txt

3 -	**Abrir o Notebook:**
	•	No Google Colab: Fazer upload do arquivo .ipynb.
	•	Ou rodar localmente com Jupyter Notebook.
