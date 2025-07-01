
---

## 🚀 Tecnologias Utilizadas

| Ferramenta           | Finalidade                          |
|----------------------|-------------------------------------|
| Python 3.10+         | Linguagem principal                 |
| Pandas / NumPy       | Manipulação de dados                |
| Scikit-learn         | Pré-processamento e árvore          |
| TensorFlow / Keras   | Rede Neural Multicamadas            |
| Matplotlib / Seaborn | Visualizações                       |
| Google Colab         | Execução interativa                 |
| NASA Exoplanet API   | Fonte de dados reais                |

---

## 📊 Dados Utilizados

- Origem: [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu/)
- Filtro: Planetas candidatos com **período orbital > 300 dias** e **raio < 2 RJ**
- Atributos usados:
  - `koi_period` (período orbital)
  - `koi_prad` (raio planetário)
  - `koi_srad` (raio da estrela)
  - `koi_steff` (temperatura efetiva da estrela)

---

## 🧠 Modelos Aplicados

### 🔹 Clusterização KMeans

- Objetivo: Agrupar exoplanetas com base em semelhança física
- Resultados: Clusters interpretáveis visualmente

### 🔹 Rede Neural Multicamadas (MLP)

- Arquitetura: `Input → Dense(32) → Dropout → Dense(32) → Output(3)`
- Acurácia final de validação: **~88%**
- Técnicas aplicadas:
  - Normalização (`StandardScaler`)
  - `Dropout`, `BatchNormalization`
  - `EarlyStopping` para evitar overfitting

![Acurácia da Rede Neural](assets/plot_accuracies.png)

---

## 🔬 Possíveis Expansões

- Aplicação em dados do TESS e K2
- Modelos mais avançados como XGBoost ou Autoencoders
- Dashboard com Gradio ou Streamlit
- Explicabilidade com SHAP / LIME
- Automação com agentes e APIs

---

## ▶️ Execute Agora no Google Colab

[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SEU_USUARIO/exoplanet-ia-classification/blob/main/exoplanet_classification.ipynb)

---

## 📦 Instalação local

```bash
git clone https://github.com/SEU_USUARIO/exoplanet-ia-classification.git
cd exoplanet-ia-classification
pip install -r requirements.txt
