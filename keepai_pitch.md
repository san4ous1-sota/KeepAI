# KeepAI — Presentation Speech
### *For potential buyers / investors*

---

## Opening

Good [morning / afternoon].

Thank you for your time today.

I'd like to introduce you to **KeepAI** — a privately deployed, AI-powered knowledge assistant built specifically for vessel and maritime operations teams.

The core idea is simple: **your crew already has all the knowledge they need — it's locked inside hundreds of PDFs, Word documents, procedures, handover notes, and technical manuals.** KeepAI makes that knowledge instantly searchable and conversational, without sending a single byte to any cloud provider.

---

## The Problem

Let me paint a picture you may recognise.

An engineer on night watch needs to check a maintenance procedure for a specific piece of equipment. He opens the shared drive, digs through folders, finds three versions of the same document, and spends twenty minutes reading through it to find the one paragraph that answers his question.

Or worse — a new officer joins the vessel. He doesn't know where anything is stored. He asks a colleague, who is busy. The knowledge exists, but it's **invisible**.

This happens hundreds of times a week across every vessel in a fleet. Time is lost. Mistakes are made. Critical information stays buried.

**KeepAI solves this.**

---

## What Is KeepAI?

KeepAI is a **self-hosted AI assistant** that runs entirely on your own server or vessel hardware — no internet connection required, no data leaves your network.

You upload your documents once. KeepAI indexes them. From that point on, anyone on the vessel can simply **ask a question in plain language** and get an accurate, sourced answer within seconds.

It works like a conversation. You type: *"What is the procedure for testing the emergency fire pump?"* — and KeepAI reads through all relevant documents, finds the answer, and tells you exactly where it came from.

---

## Key Features

### 1. Natural Language Chat with Document Sources

The heart of KeepAI is the chat interface. Users ask questions the same way they would ask a colleague. The system uses a technique called **Retrieval-Augmented Generation** — it doesn't guess or hallucinate. It retrieves real content from your actual documents, and the AI formulates a clear answer based only on what is written there.

Every answer comes with **source references** — you can see exactly which document and which section was used to generate the response.

### 2. Department-Based Document Organisation

Documents are organised by department: **General, Deck, Engine, Electrical, HSE, and Store**.

When a user asks a question, the system can be set to search only within the relevant department. An electrical engineer asking about a fault won't get results from HSE procedures or deck logs — he gets targeted, relevant answers from his own domain.

### 3. Equipment Tagging

Documents can be tagged to specific equipment — a crane, a generator, a specific pump. When a user asks about that equipment, KeepAI prioritises the manuals and procedures tagged to it. This is especially powerful for maintenance queries.

### 4. Multiple Document Types

The system handles the full range of maritime documentation:
- **Procedures** and **troubleshooting guides**
- **Handover notes**
- **Technical manuals**
- **Reports**
- PDF, Word documents, Excel spreadsheets, plain text, and Markdown — all processed automatically.

### 5. Fully Offline — No Cloud Dependency

This is a critical point. **KeepAI runs entirely on your own infrastructure.** The AI model runs locally via Ollama. The vector database, the document store, the user database — everything is on your machine.

There is no subscription to an external AI service. There is no monthly API bill that grows with usage. There is no risk of your confidential technical documents or operational data leaving the vessel.

Once deployed, KeepAI works at anchor, at sea, in port — **anywhere, regardless of internet connectivity.**

### 6. Role-Based User Access

KeepAI has a built-in user management system with roles. Standard crew members can search and chat. Management users can upload and delete documents. Administrators have full control over the system — including settings, user accounts, and maintenance tools.

### 7. Admin and Maintenance Tools

For the system administrator, KeepAI provides:
- A **document management panel** with department tabs, search, and bulk actions including batch delete
- An **Admin Preview** to inspect how any document was parsed and indexed
- A **Vector DB maintenance panel** to scan for and remove orphaned or stale data
- **System monitoring** showing collection statistics
- **Automatic backups** with one-click restore
- A **Retrieval Test Bench** — a dry-run tool that lets administrators test exactly how the AI would respond to any query, before users ever send it

### 8. Configurable Intelligence

KeepAI is not a fixed, one-size-fits-all system. Administrators can configure:
- The **answer quality / depth** slider — from fast, concise responses to deep, comprehensive searches
- Custom **workspace modes** that define which document collections are searched together
- Custom **output formats** — for example, a "timeline" format for incident investigations, or a "checklist" format for procedures
- **Investigation presets** for common operational scenarios
- **Semantic answer caching** — repeated questions are answered instantly from cache, reducing system load

---

## Deployment

KeepAI is deployed using **Docker Compose** — a standard, industry-proven container technology. Setup on a vessel server, a shore-based fleet server, or a dedicated onboard PC takes less than an hour.

The system consists of four containers:
- The **backend API** (Python / FastAPI)
- The **frontend** (React web interface, accessible from any browser on the local network)
- The **document parsing worker** (handles complex PDFs and Word files with high accuracy)
- The **local AI model** (Ollama — runs on CPU, no GPU required)

No cloud accounts. No vendor lock-in. **You own the system completely.**

---

## Who Is This For?

KeepAI is built for:
- **Vessel operators** who want to digitalise and make accessible their technical documentation library
- **Fleet management companies** who want to standardise knowledge access across multiple vessels
- **Ship management companies** who handle ISM documentation, procedures, and compliance records
- **Offshore operations** where internet connectivity is unreliable or non-existent

---

## The Value Proposition

Let me be direct about the value.

Every vessel carries years of accumulated knowledge — procedures refined through experience, handover notes written by skilled officers, manuals for every piece of equipment on board. Today, most of that knowledge is practically inaccessible at the moment it's needed most.

KeepAI turns that static archive into a **live, searchable, conversational resource** — available to every crew member, at any hour, in any language they choose to type in.

The return is measured in **time saved, errors avoided, and faster onboarding** for new crew members. More broadly, it reduces the risk of operational incidents caused by missing or hard-to-find procedural information.

---

## Closing

KeepAI is production-ready. It is running today on real hardware, handling real maritime documentation.

We are looking for partners who understand that **knowledge management is an operational safety issue**, not just a convenience — and who want a solution that respects their data sovereignty, fits within their existing IT infrastructure, and delivers immediate, measurable value to their crews.

I would be happy to walk you through a live demonstration, or to discuss how KeepAI could be customised and deployed for your specific fleet or operation.

Thank you.

---

*Estimated speaking time: approximately 6–7 minutes at a comfortable pace.*
