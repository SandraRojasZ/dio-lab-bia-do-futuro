# 🤖 Athena - Agente Financeiro Educativo

> 🏆 Projeto desenvolvido para o desafio **"Criando um Agente Financeiro com IA"** da DIO.

A **Athena** não é apenas um chatbot; é uma **educadora financeira pessoal**. Diferente de assistentes que apenas mostram saldos ou sugerem investimentos cegamente, a Athena utiliza os dados reais do cliente para **ensinar** conceitos financeiros, explicar o comportamento de gastos e promover a educação financeira sem riscos de recomendações inadequadas.

---

## 💡 O Problema e a Solução

Muitas pessoas têm dificuldade em entender conceitos como "CDI", "Selic" ou "Reserva de Emergência", mesmo tendo acesso aos dados bancários.

A **Athena** resolve isso atuando como uma "professora particular":
1.  **Contextualiza:** Explica o que é 100% do CDI usando o saldo atual da conta do usuário como exemplo.
2.  **Analisa:** Identifica gargalos no orçamento (ex: gastos excessivos com moradia) baseando-se no histórico de transações.
3.  **Protege:** Possui travas de segurança rigorosas (Anti-Alucinação) para **jamais** recomendar compras de ativos específicos, mantendo o foco puramente educativo.

---

## 🛠️ Tecnologias Utilizadas

O projeto foi construído utilizando uma stack moderna e acessível:

* **Linguagem:** [Python](https://www.python.org/)
* **Interface:** [Streamlit](https://streamlit.io/) (para um chat interativo e fluido)
* **Inteligência Artificial:** Modelo Local via [Ollama](https://ollama.com/) (Llama 3 ou compatível)
* **Processamento de Dados:** [Pandas](https://pandas.pydata.org/)
* **Integração:** REST API (Requests)

---

## 📂 Estrutura do Projeto

```bash
📁 lab-agente-financeiro/
│
├── 📁 data/                  # "Core Banking" Simulado
│   ├── historico_atendimento.csv
│   ├── perfil_investidor.json
│   ├── produtos_financeiros.json
│   └── transacoes.csv
│
├── 📁 docs/                  # Documentação do Processo
│   ├── 01-documentacao-agente.md     # Persona e Arquitetura
│   ├── 02-base-conhecimento.md       # Estrutura dos dados
│   ├── 03-prompts.md                 # Engenharia de Prompt (System Prompt)
│   ├── 04-metricas.md                # Testes de assertividade
│   └── 05-pitch.md                   # Roteiro de apresentação
│
├── 📁 src/                   # Código Fonte
│   └── app.py                # Aplicação principal (Chatbot)
│
└── 📄 README.md              # Documentação principal