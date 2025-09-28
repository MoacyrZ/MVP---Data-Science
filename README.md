# 🎸 Classificação de Guitarras com Deep Learning

Este projeto foi desenvolvido como **MVP da disciplina de Data Science da PUC-Rio**.  
O objetivo é treinar um modelo capaz de **classificar diferentes tipos de guitarras a partir de imagens**, utilizando técnicas de **transfer learning** com a MobileNetV2.

---

## 📂 Estrutura do Projeto
- `mvp_moacyr_zanoni.ipynb` → Notebook principal com todo o desenvolvimento, treinamentos, análises e conclusões.  
- `dataset.zip` → Conjunto de imagens organizado em pastas por classe.  
- `class_names.json` → Arquivo com os nomes das classes (gerado pelo notebook).  
- `modelo_guitarras_mobilenetv2.keras` → Modelo treinado salvo (gerado pelo notebook).  

---

## 🚀 Execução
Você pode rodar o notebook diretamente no Google Colab:  

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/MoacyrZ/MVP---Data-Science/blob/main/mvp_moacyr_zanoni.ipynb
)

O dataset é carregado automaticamente a partir do GitHub:  
[Dataset.zip (raw)](https://raw.githubusercontent.com/MoacyrZ/MVP---Data-Science/main/dataset.zip)

---

## 📊 Metodologia
- **Divisão dos dados:** 70% treino, 20% validação e 10% teste.  
- **Pré-processamento:** normalização + data augmentation (apenas no treino).  
- **Modelo:** MobileNetV2 pré-treinada no ImageNet.  
- **Treinamento:**  
  - Fase 1: base congelada.  
  - Fase 2: fine-tuning nas últimas 50 camadas.  
- **Avaliação:** métricas de acurácia, F1-score macro, matriz de confusão e classification report.  

---

## 📌 Resultados
No conjunto de **teste (10%)**, o modelo alcançou:  
- **Acurácia:** 75,59%  
- **F1-score macro:** 0.80  

---

## ✅ Conclusões
- O modelo conseguiu classificar guitarras com bom desempenho.  
- Principais limitações: dataset pequeno e desbalanceado.  
- Próximos passos:  
  - Expandir o dataset.  
  - Testar arquiteturas mais avançadas (EfficientNet, Vision Transformers).  
  - Explorar balanceamento de classes.  

---

## 👨‍💻 Autor
**Moacyr Zanoni**  
[MVP - Data Science](https://github.com/MoacyrZ/MVP---Data-Science)
