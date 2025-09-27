# MVP | Preditor de Satisfação do Cliente (NPS) para E-commerce

Projeto para classificar interações de clientes em **Detrator**, **Neutro** ou **Promotor** e apoiar ações de CRM/marketing.

## 🎯 Objetivo
- Identificar o nível de satisfação (NPS) em cada evento de compra/interação.
- Priorizar campanhas de retenção e indicação com base na classe prevista.
- Entregar um MVP simples, reprodutível e pronto para piloto.

## 📊 O que foi feito
- **Exploração e limpeza** dos dados (duplicatas/valores inválidos).
- **Criação do alvo** (Detrator/Neutro/Promotor) a partir da probabilidade original.
- **Divisão treino/teste** com estratificação.
- **Modelagem**: Regressão Logística (baseline) e **Random Forest**.
- **Avaliação** com relatório de classificação e matriz de confusão.
- **Entrega**: artefatos para inferência + monitoramento básico.

## 🏁 Resultados (teste)
- **Modelo vencedor**: **Random Forest (balanced)**
- **Accuracy**: **0,907** | **F1-macro**: **0,883**
- **F1 (Neutro)**: **0,804**
- Principais sinais: **sentimento da review**, **rating do produto**, **histórico de produtos similares**.

## 🛠️ Tecnologias
- Python • Pandas • NumPy • Matplotlib
- Scikit-learn (Pipeline, OneHotEncoder, Logistic Regression, Random Forest)

## ▶️ Como rodar
1. Abrir o notebook e executar **Restart & Run All**.
2. Artefatos gerados:
   - `mvp_model.joblib` (modelo pronto para uso)
   - `mvp_metadata.json` (colunas, classes, métricas)
   - `monitor_baseline.json` e `pred_log.parquet` (monitoramento)

## 📁 Arquivo do Projeto
- Notebook: `MVP_NPS_Completo_2.ipynb`

## 👤 Autoria
**Fabiane Silveira**


🔗 

## 👤 Licença / Autoria

**Fabiane Silveira**  

PUC-RIO  

Curso: CIÊNCIA DE DADOS E ANALYTICS

Sprint: Machine Learning & Analytics

Projeto acadêmico para avaliação; uso interno/educacional.

