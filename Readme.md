# 📊 Dataset — Social Media Ads Campaign  

Este conjunto de dados é **sintético** e foi criado para simular o desempenho de campanhas publicitárias em redes sociais (ex.: Facebook, Instagram). Ele é composto por **quatro tabelas principais**, todas interligadas por **chaves primárias e estrangeiras**.  

---

## 📂 Estrutura dos Dados  

### 1. `users.csv`  
Informações de usuários que interagiram com campanhas.  
- **user_id** — identificador único do usuário  
- **age** — idade do usuário  
- **gender** — gênero (ex.: Male, Female, Other)  
- **country** — país de origem  
- **location** — localização mais detalhada (cidade/região)  
- **interests** — interesses do usuário (ex.: esportes, música, tecnologia)  

---

### 2. `campaigns.csv`  
Dados das campanhas de marketing.  
- **campaign_id** — identificador único da campanha  
- **name** — nome da campanha  
- **budget** — orçamento total da campanha  
- **start_date** — data de início  
- **end_date** — data de término  

---

### 3. `ads.csv`  
Anúncios vinculados às campanhas.  
- **ad_id** — identificador único do anúncio  
- **campaign_id** — chave estrangeira para a campanha  
- **content** — descrição ou tipo do criativo (ex.: imagem, vídeo, texto)  
- **target_age** — faixa etária alvo  
- **target_gender** — gênero alvo  
- **target_interests** — interesses alvo  

---

### 4. `ad_events.csv`  
Registro de interações dos usuários com os anúncios (funil de conversão).  
- **event_id** — identificador único do evento  
- **user_id** — chave estrangeira para `users`  
- **ad_id** — chave estrangeira para `ads`  
- **event_type** — tipo de evento (Impression, Click, Purchase, etc.)  
- **timestamp** — momento em que ocorreu o evento  

---

## 🔗 Relacionamentos Entre Tabelas  
- `users` ↔ `ad_events` (via **user_id**)  
- `ads` ↔ `ad_events` (via **ad_id**)  
- `campaigns` ↔ `ads` (via **campaign_id**)  

---

## 🚀 Possibilidades de Análise  
- Explorar o **funil de conversão** (impressão → clique → compra)  
- Avaliar quais campanhas e anúncios tiveram **melhor desempenho**  
- Analisar o impacto de **demografia e interesses** nos resultados  
- Calcular métricas como **CTR (Click-Through Rate)** e **Taxa de Conversão**  

---
