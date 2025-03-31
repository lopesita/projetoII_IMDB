# 🎬 Projeto Aplicado II - Análise de Sentimentos IMDB

Este repositório contém uma aplicação de **aprendizado de máquina supervisionado** para análise de sentimentos em avaliações de filmes da base **IMDB**. O principal objetivo é classificar os comentários como **positivos** ou **negativos** por meio de técnicas de **PLN (Processamento de Linguagem Natural)**.

---

## 📁 Estrutura do Repositório

```
Projeto-IMDB/
│
├── datasets/                  
│   └── IMDB Dataset.csv       # Base original de avaliações
│
├── notebooks/                 
│   └── Regressão_Logística_IMBD_reajustado2v.ipynb  # Notebook principal
│
├── read.me/                   
│   └── README.md              # Este arquivo de documentação
```

---

## 🔍 Etapas do Projeto

### 1. Análise Exploratória de Dados (EDA)
- Visualização da distribuição de sentimentos com `seaborn`
- Cálculo e visualização de outliers com base no comprimento das avaliações (IQR)
- Gráficos interativos com `plotly` (opcional)

### 2. Pré-Processamento de Dados
- Leitura da base com pandas
- Limpeza e normalização de textos
- Criação de variáveis auxiliares (`text_length`, `clean_review`, etc.)


- Visualização da distribuição de sentimentos com `seaborn`
- Cálculo e visualização de outliers com base no comprimento das avaliações (IQR)
- Gráficos interativos com `plotly` (opcional)

### 3. Processamento de Dados
- Mapeamento de sentimentos (`positive` → 1, `negative` → 0)
- Criação de subconjuntos filtrando outliers
- Preparação para vetorização e modelagem

---

## 📦 Bibliotecas Utilizadas

- `pandas`, `numpy`
- `matplotlib`, `seaborn`, `plotly`
- `scikit-learn`
- `mplcyberpunk` (estética visual extra)

---

## ▶️ Como Executar

Você pode abrir e executar o projeto localmente com:

```bash
jupyter notebook notebooks/Regressão_Logística_IMBD_reajustado2v.ipynb
```

Ou usar o Google Colab (recomenda-se montar o Google Drive para acessar o CSV).

---

## 👤 Autores

**Italo Aparecido Lopes**


**Gabriel Chaves Gonçalves** 
Projeto acadêmico para a disciplina **Projeto Aplicado II** no curso de Ciência de Dados.

---

## 📌 Observações

- O projeto ainda está em desenvolvimento.


---

## 💻 Execução no Google Colab

Este projeto foi executado originalmente com o Colab conectado a um **ambiente de execução local**, mas também pode ser executado diretamente no ambiente de nuvem do Google Colab. Caso escolha essa opção, siga os passos abaixo para garantir que o arquivo `IMDB Dataset.csv` seja acessado corretamente:

### Passos para montar o Google Drive no Colab:

1. **Monte seu Google Drive:**
```python
from google.colab import drive
drive.mount('/content/drive', force_remount=True)
```

2. **Defina o diretório de trabalho:**
```python
import os
os.chdir('/content/drive/MyDrive/')
```

3. **Carregue o dataset a partir do seu Drive:**
Certifique-se de que o arquivo `IMDB Dataset.csv` está dentro da pasta `MyDrive`:
```python
df = pd.read_csv("IMDB Dataset.csv")
```

> Assim, você garante que o código funcionará mesmo em um ambiente de execução hospedado pela Google.

---
