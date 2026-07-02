# Beleqet Backend — NestJS API

ይህ ፕሮጀክት በ NestJS እና በ PostgreSQL ላይ የተገነባ፣ ለ "Beleqet" የሥራ እና የፍሪላንስ መድረክ (Hiring & Freelance Platform) የተዘጋጀ ሙሉ (Production-ready) የኋላ መተግበሪያ (Backend API) ነው። ይህ መድረክ ቀጣሪዎችን እና ፈላጊዎችን በኤአይ (AI) ታግዞ የሚያገናኝ ሲሆን፣ የገንዘብ ክፍያ አስተዳደርን (Escrow) እና የስራ ፍሰት አውቶሜሽንን (Event-Driven Workflow) ያካተተ ነው።

## How to Run

```bash
# 1. Set up environment properties
cp .env.example .env
# Edit your local .env file variables (Set PORT=4002)

# 2. Orchestrate and launch all services cleanly via Docker
docker compose down
docker compose up --build