# 🎓 João — Educador Financeiro com IA

Agente conversacional educativo que ensina conceitos de finanças pessoais de forma simples, usando os dados do próprio cliente como exemplos práticos — sem recomendar investimentos.

> Projeto desenvolvido como parte do lab **"Bia do Futuro"** da [DIO](https://dio.me).

---

## 🧩 O Problema

Muitas pessoas têm dificuldade em entender conceitos básicos de finanças pessoais: reserva de emergência, tipos de investidores e como organizar os próprios gastos.

## 💡 A Solução

O **João** é um agente educativo que explica finanças de forma acessível, usando linguagem informal e exemplos personalizados — como um professor particular financeiro.

---

## 🛠️ Tecnologias

| Camada | Tecnologia |
|--------|------------|
| Interface | [Streamlit](https://streamlit.io) |
| LLM | [Ollama](https://ollama.com) (local) |
| Linguagem | Python 3 |
| Dados | JSON e CSV mockados (`/data`) |

---

## 📁 Estrutura do Projeto

```text
dio-lab-bia-do-futuro/
├── data/
│   ├── perfil_investidor.json        # Perfil e metas do cliente
│   ├── transacoes.csv                # Histórico de transações
│   ├── historico_atendimento.csv     # Histórico de atendimentos
│   └── produtos_financeiros.json     # Produtos disponíveis para ensino
├── docs/
│   ├── 01-documentacao-agente.md     # Caso de uso e arquitetura
│   ├── 02-base-conhecimento.md       # Estratégia de dados e contexto
│   ├── 03-prompts.md                 # System prompt e exemplos
│   ├── 04-metricas.md                # Avaliação e métricas de qualidade
│   └── 05-pitch.md                   # Roteiro do pitch
├── src/
│   └── app.py                        # Aplicação principal
└── README.md
```
---

## ▶️ Como Executar

**Pré-requisito:** ter o [Ollama](https://ollama.com) instalado e rodando localmente.

```bash
# 1. Clone o repositório
git clone https://github.com/makil2/dio-lab-bia-do-futuro.git
cd dio-lab-bia-do-futuro

# 2. Instale as dependências
pip install streamlit pandas requests

# 3. Execute a aplicação
streamlit run src/app.py
```

---

## 🤖 Persona do Agente

- **Nome:** João
- **Papel:** Educador financeiro
- **Tom:** Informal, didático e paciente — como um amigo que entende de finanças
- **Regras principais:**
  - ✅ Explica como os produtos financeiros funcionam
  - ✅ Usa os dados do cliente como exemplos práticos
  - ✅ Admite quando não sabe algo
  - ❌ Nunca recomenda investimentos específicos
  - ❌ Nunca responde perguntas fora do escopo financeiro

---

## 🛡️ Estratégias Anti-Alucinação

- Opera apenas com dados fornecidos no contexto
- Não acessa dados bancários reais
- Declara explicitamente suas limitações
- Não substitui profissionais certificados (CFP, CGA etc.)

---

## 📊 Métricas de Qualidade

| Métrica | O que avalia |
|---------|--------------|
| Assertividade | A resposta respondeu o que foi perguntado? |
| Segurança | O agente evitou inventar informações? |
| Coerência | A linguagem foi clara e adequada ao perfil? |

---

## 📚 Documentação Completa

Toda a documentação está na pasta [`/docs`](./docs), cobrindo arquitetura, base de conhecimento, engenharia de prompts, métricas e roteiro de pitch.

---

## 👤 Autor

Desenvolvido por **makil2** · [GitHub](https://github.com/makil2)
