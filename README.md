# 📘 Perfumes & Psicologia — Projeto Modelagem Estatística  
**Autor:** Ana Luiza Souto e Matheus Leão 

**Curso:** Modelagem Estatistica

**Dataset:** Perfume & Psychology ([Kaggle, CC BY-N](https://www.kaggle.com/datasets/priyanshubhaskar/perfume-and-psychology))

---

## 📌 Sobre o Projeto

Este repositório contém a implementação completa do projeto final, incluindo:

- **Coleta e tratamento dos dados** (3 CSVs: Brainfunc, Psycho e Compound)  
- **Análise Exploratória (EDA)** detalhada  
- **Testes estatísticos** (Spearman, ANOVA, Chi-Square quando aplicável)  
- **Modelagem de Regressão** (Linear, Múltipla, Polinomial, Ridge)  
- **Modelagem de Classificação** (Naive Bayes e Regressão Logística)  
- **Otimização** via GridSearchCV, RandomizedSearchCV e PyCaret  
- **Diagnóstico de resíduos**, multicolinearidade (VIF), normalidade e homocedasticidade  
- **Relatório final completo** com explicações das hipóteses  

O projeto segue todos os requisitos da disciplina, garantindo reprodutibilidade e clareza metodológica.

---

## 📂 Estrutura do Repositório


```
├── data/
│ └── Perfume&Psychology/
│ ├── perfume_Brainfunc.csv
│ ├── perfume_compound.csv
│ └── perfume_Psycho.csv
│
├── artifacts/
│ ├── X_all.pkl
│ ├── y_clf.pkl
│ ├── y_reg.pkl
│ ├── logistic_final.pkl
│ ├── mnb_final.pkl
│ ├── ridge_eeg_final.pkl
│ ├── classification_holdout_metrics.csv
│ └── regression_cv_metrics.csv
│
├── figures/
│ ├── h4_brainfunc_vs_textlen.png
│ └── box_brainfunc_bucket_textlen.png
│
├── notebook.ipynb # arquivo principal com toda análise
├── requirements.txt
└── README.md
```


## ⚙️ Como Executar

### 1. Criar ambiente:
```bash
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate     # Windows
```

### Instalar dependências:
```bash
pip install -r requirements.txt
```

### Abrir Jupyter Notebook:
```bash
jupyter notebook
```


### 📊 Principais Resultados
```
- Hipotese rejeitada (Spearman p=0.79, ANOVA p=0.79)
- Modelos de classificação perfomaram com F1=1.0, porém com forte indício de overfitting devido ao N reduzido (N=44).
- Modelos de regressão apresentaram R² ≈ 0, indicando ausência de relação linear robusta.
- O projeto demonstra domínio de: EDA, regressão, classificação, tuning, e diagnóstico estatístico.
```

### 📄 Licença
```
Este projeto utiliza dados sob licença CC0: Public Domain do Kaggle.
Link: https://creativecommons.org/publicdomain/zero/1.0/
```
