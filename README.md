# Detecção Preditiva de Ataques Cibernéticos: Uma Abordagem de Machine Learning

## Descrição
Este projeto tem como objetivo desenvolver um **modelo de Machine Learning** capaz de detectar intrusões cibernéticas com base em padrões de tráfego de rede e comportamento de usuários.  

Foi desenvolvido como trabalho de **final de curso na Le Wagon**, no curso de **Data Analytics**, em equipe com **Rodrigo Martins** e **Cíntia Simões**.  

Utilizamos o dataset [Cybersecurity 🪪 Intrusion 🦠 Detection Dataset](https://www.kaggle.com/datasets/dnkumars/cybersecurity-intrusion-detection-dataset/data), que contém registros de sessões de rede com informações de protocolos, tentativas de login e indicadores de ataque. O projeto inclui **análise exploratória, pré-processamento, modelagem, avaliação e dashboard interativo** para visualização de insights.

---

## Tecnologias Utilizadas
- Python (Pandas, Numpy, Scikit-learn, XGBoost, LightGBM, Matplotlib, Seaborn)  
- Google Colab (Notebooks na nuvem)  
- Looker Studio (visualização de dados)

---

## Estrutura do Projeto
- `data/` → Dados brutos e processados.  
- `notebooks/` → Notebooks de análise exploratória, pré-processamento e modelagem (Google Colab).  
- `src/` → Scripts de funções para tratamento, modelagem e avaliação.  
- `models/` → Modelos treinados no Colab (XGBClassifier e outros testados).  
- `reports/` → Gráficos, visualizações e relatórios de resultados.  
- `dashboard/` → Links ou arquivos do dashboard interativo (Looker Studio).  
- `docs/` → Referências bibliográficas e materiais complementares.

---

## Variáveis do Dataset
- `session_id`: Identificador da sessão  
- `network_packet_size`: Tamanho médio dos pacotes de rede  
- `protocol_type`: Tipo de protocolo (TCP, UDP, ICMP)  
- `login_attempts`: Número de tentativas de login  
- `session_duration`: Duração da sessão  
- `encryption_used`: Uso de criptografia (sim/não)  
- `ip_reputation_score`: Reputação do IP de origem  
- `failed_logins`: Número de falhas de login  
- `browser_type`: Navegador utilizado  
- `unusual_time_access`: Acesso em horário incomum (sim/não)  
- `attack_detected`: Variável alvo (0 = acesso legítimo, 1 = ataque)

---

## Etapas do Projeto
1. **Coleta de Dados**  
   - Dataset: [Cybersecurity Intrusion Detection Dataset](https://www.kaggle.com/datasets/dnkumars/cybersecurity-intrusion-detection-dataset/data)  
   - Formato: CSV, com registros de sessões de rede e variáveis de comportamento.

2. **Análise Exploratória e Pré-processamento**  
   - Notebook: [EDA e Preprocessamento](https://colab.research.google.com/drive/1xrLoRhMHhXFOeq-iNq4ZObZVPmuLpe4G?usp=sharing)  
   - Limpeza de dados, tratamento de valores ausentes e engenharia de features.

3. **Treinamento de Modelos de Classificação**  
   - Notebook: [Modelo de ML](https://colab.research.google.com/drive/1TXT9j1mv9K_lphKSlrmcTr8MeLW1x6eW?usp=sharing)  
   - Algoritmos testados:
     - RandomForestClassifier (Floresta Aleatória)  
     - LGBMClassifier (Máquina de Reforço de Gradiente Leve)  
     - XGBClassifier (Reforço de Gradiente Extremo)  
     - ExtraTreesClassifier (Árvores Extremamente Aleatórias)  
   - **Modelo escolhido:** XGBClassifier  
   - Objetivo: Classificação de sessões como ataque ou legítima.

4. **Avaliação de Métricas**  
   - Métricas utilizadas: Accuracy, Precision, Recall, F1-score, AUC  
   - Comparação entre modelos para seleção do melhor desempenho.

5. **Exportação do Modelo Final**  
   - Modelos treinados ficam disponíveis nos notebooks do Colab (`notebooks/`).  

6. **Dashboard Interativo**  
   - [Looker Studio Dashboard](https://lookerstudio.google.com/reporting/f113278d-5a0b-47e0-8083-f71180fe5338)  
   - Visualização de insights e resultados do modelo.

---

## Referências
- [Dataset no Kaggle](https://www.kaggle.com/datasets/dnkumars/cybersecurity-intrusion-detection-dataset/data)  
- [Notebook de Análise Exploratória e Pré-processamento](https://colab.research.google.com/drive/1xrLoRhMHhXFOeq-iNq4ZObZVPmuLpe4G?usp=sharing)  
- [Notebook de Modelagem de ML](https://colab.research.google.com/drive/1TXT9j1mv9K_lphKSlrmcTr8MeLW1x6eW?usp=sharing)  
- [Looker Studio Dashboard](https://lookerstudio.google.com/reporting/f113278d-5a0b-47e0-8083-f71180fe5338)

---

## Contato
- [LinkedIn](https://www.linkedin.com/in/ingrid-pessoa-bighetti-79849650/)  
- [E-mail](mailto:ingridpessoa1992@gmail.com)
