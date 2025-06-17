# Challenge-TelecomX

# 📊 Análise de Evasão de Clientes - Telecom X

Este projeto tem como objetivo analisar os dados de clientes da empresa **Telecom X** com foco no problema de **evasão de clientes (Churn)**. Através de um processo completo de limpeza, tratamento e exploração dos dados, foram extraídos insights valiosos que podem ajudar a empresa a **reduzir a saída de clientes** e **aumentar a retenção**.

---

## 🧠 Introdução

A evasão de clientes é um dos maiores desafios no setor de telecomunicações. Manter um cliente custa menos do que conquistar um novo. Este projeto tem como missão **descobrir padrões nos dados de clientes evadidos** e propor ações com base nessas descobertas.

---

## 🧹 Etapas de Limpeza e Tratamento de Dados

- Importação dos dados a partir de um arquivo `.json`.
- Normalização da estrutura com `pandas.json_normalize`.
- Conversão de tipos numéricos e correção de dados inconsistentes.
- Padronização textual: minúsculas, sem espaços e com underscore (`snake_case`).
- Substituição de valores nulos e transformação de variáveis categóricas em numéricas.
- Criação de nova feature: `contas_diarias` = cobrança mensal / 30.

---

## 📊 Análise Exploratória de Dados (EDA)

### 📌 Tipo de Contrato

| Tipo               | Taxa de Churn |
|--------------------|---------------|
| Mensal             | **41,3%**     |
| 1 ano              | 10,9%         |
| 2 anos             | 2,8%          |

📉 Contratos mensais estão fortemente associados à evasão.

---

### 📌 Método de Pagamento

| Método                  | Taxa de Churn |
|-------------------------|---------------|
| Electronic Check        | **43,8%**     |
| Mailed Check            | 18,5%         |
| Bank Transfer (Auto)    | 16,2%         |
| Credit Card (Auto)      | 14,8%         |

💳 Pagamentos automáticos são mais estáveis.

---

### 📌 Serviços Adicionais

| Serviço              | Taxa de Churn |
|----------------------|----------------|
| Sem Backup Online    | 38,7%          |
| Com Backup Online    | 20,9%          |
| Sem Suporte Técnico  | 30,2%          |
| Com Suporte Técnico  | 14,7%          |
| Sem Streaming TV     | 23,6%          |
| Com Streaming TV     | 29,2%          |

🛡️ Serviços extras ajudam a reter o cliente.

---

### 📌 Perfil Familiar

| Situação                | Taxa de Churn |
|-------------------------|---------------|
| Sem Companheiro(a)      | 32,0%         |
| Com Companheiro(a)      | 19,0%         |
| Sem Dependentes         | 30,3%         |
| Com Dependentes         | 14,9%         |

👪 Clientes com família têm menor propensão ao cancelamento.

---

### 📌 Tipo de Internet

| Tipo          | Taxa de Churn |
|---------------|---------------|
| Fiber Optic   | **40,6%**     |
| DSL           | 18,4%         |
| Sem Internet  | 7,1%          |

⚠️ A tecnologia de fibra óptica está associada a maior churn — merece investigação.

---

### 📌 Gênero

| Gênero     | Taxa de Churn |
|------------|---------------|
| Feminino   | 26,0%         |
| Masculino  | 25,0%         |

📎 Sem diferença significativa entre os gêneros.

---

## 🧾 Conclusões

- Contratos mensais e pagamentos via **electronic check** são os maiores vilões da retenção.
- Clientes **com serviços adicionais** e **laços familiares** tendem a permanecer mais tempo.
- **Alta cobrança mensal** e **baixo tempo de casa** também aparecem ligados à evasão.

---

## 💡 Recomendações

1. **Incentivar migração para contratos de longo prazo**.
2. **Campanhas para migrar clientes de electronic check para métodos automáticos**.
3. **Oferecer pacotes com serviços adicionais gratuitos nos primeiros meses**.
4. **Focar nos clientes novos** com estratégias de boas-vindas e onboarding.
5. **Analisar clientes com cobrança mensal alta** e oferecer alternativas mais econômicas.

---

## 📁 Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

---

## 📌 Resultado Esperado

Com as estratégias baseadas nos dados analisados, espera-se **reduzir a taxa de evasão** e aumentar a fidelização dos clientes, tornando a Telecom X mais competitiva e lucrativa.

---

**Autora**: Tayara 👩‍💻  
**Objetivo**: Aprendizado prático em análise de dados, churn e tomada de decisão com base em evidências.  

