# 💰 Vendas IA + Pix

Sistema de registro de vendas por voz integrado ao **Google Sheets**, **Google Apps Script**, **Gemini IA** e **Pix**.

O vendedor pode falar a venda naturalmente, por exemplo:

> "João comprou dois pastéis e uma Coca por trinta reais"

A inteligência artificial interpreta a fala e transforma em dados estruturados.

Depois, basta clicar em:

**💳 SALVAR E GERAR PIX**

O sistema salva a venda no Google Sheets e gera o Pix com valor correspondente.

---

## 🚀 Funcionalidades

- 🎤 Registro de vendas por voz
- 🤖 Interpretação automática usando Gemini
- 👤 Identificação do cliente
- 🛒 Identificação dos produtos
- 🔢 Quantidade de produtos
- 💰 Identificação do valor da venda
- 📝 Descrição automática
- 📊 Registro automático no Google Sheets
- 💳 Geração de Pix Copia e Cola
- 📱 Geração de QR Code Pix
- 📋 Botão para copiar o Pix
- ❌ Cancelamento da venda
- 📈 Total de vendas do dia
- 💚 Menu próprio dentro do Google Sheets
- 🌐 Interface hospedada no GitHub Pages
- 🔐 Chave Gemini armazenada no Apps Script
- 📱 Interface adaptada para celular e computador

---

# 🧠 Como funciona

A arquitetura do projeto é:

```text
┌──────────────────────┐
│      VENDEDOR        │
│                      │
│ 🎤 Fala a venda      │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│      GitHub Pages    │
│                      │
│     index.html       │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│   Google Apps Script │
│                      │
│      Code.gs         │
└──────────┬───────────┘
           │
           ├──────────────► Gemini IA
           │
           ▼
┌──────────────────────┐
│    Google Sheets     │
│                      │
│      Vendas          │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│         PIX          │
│                      │
│ QR Code + Copia Cola │
└──────────────────────┘
