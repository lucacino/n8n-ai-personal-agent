# n8n AI Agent — Personal Assistant 🤖

> Agente AI personale costruito su n8n che riceve comandi via Telegram e gestisce autonomamente email, calendario e rubrica contatti.

**IT** | Progetto di AI Agents realizzato nell'ambito del Master in Data Science, Analytics e AI @ Start2Impact University.

---

## Obiettivo / Objective

**IT:** Costruire un agente AI personale e funzionante su n8n, piattaforma no-code per l'automazione dei workflow. L'agente riceve comandi tramite Telegram — sia messaggi testuali che vocali — e gestisce autonomamente email, calendario ed rubrica contatti integrando cinque servizi diversi.

**EN:** Build a fully functional personal AI agent on n8n, a no-code workflow automation platform. The agent receives commands via Telegram (text and voice) and autonomously manages emails, calendar events, and contacts by integrating five different services.

---

## Funzionalità / Features

- Ricezione comandi via **Telegram** (testo e messaggi vocali)
- Consultazione rubrica contatti su **Airtable**
- Invio email tramite **Gmail**
- Creazione eventi su **Google Calendar**
- Elaborazione del linguaggio naturale tramite **OpenAI**

---

## Architettura del Workflow

```
Telegram (input testuale / vocale)
        ↓
    OpenAI (elaborazione linguaggio naturale)
        ↓
  ┌─────┴──────┬──────────────┐
Airtable    Gmail      Google Calendar
(rubrica)  (email)      (eventi)
```

L'agente interpreta il comando ricevuto via Telegram, decide autonomamente quale tool utilizzare e restituisce una risposta all'utente nella stessa chat.

---

## Stack Tecnologico / Tech Stack

- **n8n** — orchestrazione del workflow (no-code)
- **Telegram Bot API** — interfaccia di input (testo + voce)
- **OpenAI API** — elaborazione linguaggio naturale e decision making
- **Airtable** — database rubrica contatti
- **Gmail API** — invio email
- **Google Calendar API** — creazione eventi

---

## Struttura del Repository

```
n8n-ai-personal-agent/
├── README.md
└── presentation/
    └── Progetto_Agenti_AI_di_Luca_Cino.pdf
```

---

## Note

Il workflow n8n non è esportabile come file di codice tradizionale. Per replicare l'agente è necessario ricostruire il workflow su n8n seguendo l'architettura descritta e configurare le credenziali per ciascun servizio (Telegram, OpenAI, Airtable, Gmail, Google Calendar).

---

## Autore / Author

**Luca Cino** — [LinkedIn](https://www.linkedin.com/in/lucacino) | [GitHub](https://github.com/lucacino)

Master Professionale in Data Science, Analytics e AI @ Start2Impact University
