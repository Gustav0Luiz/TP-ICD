# 📊 Dataset — The Complete Pokémon Dataset  

Este conjunto de dados contém informações sobre **802 Pokémon** das sete primeiras gerações da franquia. Ele inclui estatísticas base, características físicas, classificações e atributos relacionados ao jogo. 

---

## 📂 Estrutura dos Dados  

### 1. Identificação  
- **name** — Nome em inglês do Pokémon  
- **japanese_name** — Nome original em japonês  
- **pokedex_number** — Número de registro no Pokédex Nacional  
- **generation** — Geração em que o Pokémon foi introduzido (1 a 7)  
- **is_legendary** — Indica se o Pokémon é lendário (1) ou não (0)  

---

### 2. Tipos e Classificação  
- **type1** — Tipo primário do Pokémon (ex.: Fire, Water, Grass)  
- **type2** — Tipo secundário do Pokémon (pode estar vazio)  
- **classification** — Classe do Pokémon, conforme descrito na Pokédex  
- **abilities** — Lista de habilidades possíveis  

---

### 3. Atributos Físicos  
- **height_m** — Altura em metros  
- **weight_kg** — Peso em quilogramas  
- **percentage_male** — Percentual da espécie que é macho (vazio se sem gênero)  

---

### 4. Reprodução e Crescimento  
- **capture_rate** — Taxa de captura do Pokémon  
- **base_egg_steps** — Número de passos para chocar o ovo  
- **experience_growth** — Curva de crescimento de experiência  
- **base_happiness** — Felicidade inicial do Pokémon  

---

### 5. Estatísticas de Batalha  
- **hp** — Pontos de vida base  
- **attack** — Ataque base  
- **defense** — Defesa base  
- **sp_attack** — Ataque especial base  
- **sp_defense** — Defesa especial base  
- **speed** — Velocidade base  
- **against_*** — Colunas que indicam a vulnerabilidade ou resistência contra cada tipo (ex.: `against_fire`, `against_water`, etc.), onde valores > 1 indicam fraqueza e < 1 resistência.  

---

## 🚀 Objetivo do Trabalho  

O objetivo deste projeto é aplicar o **ciclo completo de ciência de dados** sobre este dataset, explorando suas características, realizando testes estatísticos e construindo modelos de predição e classificação.  

---

# ❓ Perguntas de Pesquisa  

### Pergunta 1 — Classificação  
**É possível prever se um Pokémon é lendário ou não com base em seus atributos (status base, altura, peso, tipos)?**  

### Pergunta 2 — Regressão  
**A taxa de captura de um Pokémon pode ser prevista a partir de suas estatísticas base (HP, defesa, ataque, etc.)?**  

### Pergunta 3 — Testes de Hipótese  
**Pokémons do tipo Dragão têm estatísticas de ataque significativamente maiores do que Pokémons de outros tipos?**  

### Pergunta 4 — Taxa de Captura  
**A taxa de captura de um Pokémon está relacionada às suas estatísticas base (como HP e defesa)?**  
