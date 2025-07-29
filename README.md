# 🏙️ Classificação de Faixas de Preço de Aluguel na Cidade de São Paulo

Projeto de aprendizado de máquina com foco na **classificação de valores de locação residencial** na cidade de São Paulo, utilizando técnicas de *ensemble learning* e engenharia de atributos geográficos e socioeconômicos.

Este repositório é resultado de um trabalho acadêmico desenvolvido em grupo na Universidade Federal de São Carlos (UFSCar), com **ênfase nas contribuições técnicas e analíticas de Pedro Henrique Ghiotto**.

---

## ✨ Destaques do Projeto

- 🔍 Aplicação de técnicas de **Machine Learning supervisionado** para prever faixas de aluguel residencial.
- 🧠 Combinação de diversos modelos por meio de **técnicas de ensemble** como *votação simples* e *votação ponderada*.
- 🗺️ Transformação avançada de atributos de localização em **índices socioeconômicos (IDH por subprefeitura)**, usando APIs de geolocalização.
- 📊 Validação cruzada com **10 folds estratificados** para garantir consistência na avaliação dos modelos.
- 📈 Métricas avaliadas: acurácia balanceada, matriz de confusão, ROC e relatórios de classificação.

---

## 📌 Objetivo

Criar um modelo de classificação capaz de estimar **faixas de preço de aluguel** com base em atributos de imóveis, incluindo dados espaciais e socioeconômicos, contribuindo para a tomada de decisão de locadores e locatários.

---

## 🔧 Tecnologias e Bibliotecas Utilizadas

- Python
- Scikit-learn
- Pandas
- Numpy
- Google Colab
- Nominatim (OpenStreetMap Geocoding API)

---

## 📁 Dados

- Dataset original disponível no [Kaggle](https://www.kaggle.com/datasets/renatosn/sao-paulo-housing-prices)
- Dados processados contendo:
  - Localização → Subprefeitura → IDH
  - Área, número de quartos, tipo de imóvel, total do aluguel
  - Classe alvo: 4 faixas de valores totais

---

## 🧪 Modelos Treinados

| Modelo                   | Participação no Ensemble |
|--------------------------|--------------------------|
| K-Nearest Neighbors      | ✔️                       |
| Random Forest            | ✔️                       |
| Decision Tree            | ✔️                       |
| SVM                      | ✔️ (peso 2)              |
| Gradient Boosting        | ✔️ (peso 4)              |
| Naive Bayes              | ❌ (excluído / peso -3)  |
| MLP (Rede Neural)        | ✔️ (peso 2)              |

**Melhor Resultado:**  
Ensemble com votação ponderada → **Balanced Accuracy: 0.647**

---

## 📌 Contribuições Pessoais

Embora o projeto tenha sido realizado em grupo, esta versão do repositório destaca a atuação de **Pedro Henrique Ghiotto**, que contribuiu de forma ativa nas seguintes frentes:

- 🔁 Implementação do pipeline de transformação de localização → IDH
- 🔬 Análise crítica dos resultados e avaliação dos modelos
- 🧩 Implementação do ensemble com votação ponderada
- 📈 Visualização e análise de curvas ROC, matrizes de confusão e métricas de performance
- 💡 Discussões estratégicas para definição dos pesos no ensemble

---

## 📚 Documentação e Relatório

O relatório completo do projeto com todas as etapas pode ser acessado neste repositório: `ClassificacaoPrecoLocacaoSPRelatorio.pdf`

---

## 📬 Contato

**Pedro Henrique Ghiotto**  
Estudante de Ciência da Computação – UFSCar  
📧 pedroghiotto@estudante.ufscar.br  
🔗 [LinkedIn](www.linkedin.com/in/pedro-ghiotto-871623180)

---

> Este projeto reflete minha dedicação em aplicar ciência de dados de forma prática e relevante, unindo análise de dados, engenharia de atributos e modelos de machine learning para resolver problemas do mundo real.
