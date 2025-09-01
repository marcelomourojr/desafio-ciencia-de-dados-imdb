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
	Relação entre **número de votos** e **faturamento**: filmes com maior engajamento tendem a faturar mais.
   	Distribuição de notas do IMDb concentrada entre 6 e 8.
   	Insights de palavras-chave na sinopse (Overview) para identificação de gênero.

---

2. **Respostas às Perguntas:**

**a) Qual filme você recomendaria para uma pessoa que você não conhece?**  
🎬 *The Shawshank Redemption* (Nota IMDb: **9.3**) Eu recomendaria o filme com a maior nota

---

**b) Quais são os principais fatores relacionados com alta expectativa de faturamento?**  
📈 O principal fator está relacionado ao número de votos, quanto maior o número de votos, naturalmente será maior o faturamento

---

**c) Quais insights podem ser tirados da coluna Overview?**  
📖 A sinopse pode ser usada para:
É possível usá-la para extrair palavras chave e entender melhor o gênero de cada filme.
Como "war", "battle" e "soldier" podem indicar filmes de guerra, e "love", "romance" e "relationship" podem indicar filmes românticos.

---

3. **Previsão da Nota IMDb**  
- Tipo de problema: **Regressão**  
- Variáveis escolhidas: `Meta_score`, `No_of_Votes`, `Runtime`  
- Modelo: **Regressão Linear** (pela simplicidade e boa interpretabilidade)  
- Métricas de avaliação:
  - **EAM (Erro Absoluto Médio)** ≈ 0.19  
  - **REQM (Raiz do Erro Quadrático Médio)** ≈ 0.23  


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
