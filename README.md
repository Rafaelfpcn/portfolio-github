# 🚀 Estratégia de Portfólio GitHub & Projeto Flagship (CortexRAG)

Este diretório contém a estratégia completa de posicionamento para vagas técnicas de alto nível (Pleno/Sênior) e o código funcional do projeto carro-chefe.

---

## 📂 Conteúdo Deste Diretório

1. 📄 **[ESTRATEGIA_PORTFOLIO_GITHUB.md](./ESTRATEGIA_PORTFOLIO_GITHUB.md)**  
   Guia completo contendo:
   - A Tríade de Contratação (Live Demo, CI/CD, Documentação de Decisões)
   - A Trinca de Repositórios Pinados (Tabelas comparativas e valor para o recrutador)
   - Especificação técnica profunda da arquitetura do Flagship (CortexRAG)
   - Diagrama de Arquitetura em Mermaid.js
   - O plano de execução em 5 Sprints
   - Dicas práticas para entrevistas técnicas

2. 🧠 **[cortex-rag/](./cortex-rag)**  
   Código-fonte completo, funcional e testado do projeto **CortexRAG**:
   - **Backend:** FastAPI (Python assíncrono), Pydantic v2, SQLAlchemy 2.0, pgvector / SQLite, Redis, Token Bucket Rate Limiter, Cache Semântico e Ingestão com RRF.
   - **Frontend:** Next.js 15 (App Router, Tailwind, Shadcn UI) + Web Client Dark Mode nativo.
   - **Infraestrutura:** `docker-compose.yml`, Dockerfiles, `.env.example`, `.github/workflows/ci.yml`.
   - **Testes:** Suíte completa com `pytest-asyncio` e cobertura de código (100% de sucesso nos testes).

---

## ⚡ Como Iniciar Rapidamente o CortexRAG

```powershell
cd cortex-rag\backend
python -m venv .venv
.\.venv\Scripts\activate
pip install -r requirements.txt
uvicorn app.main:app --port 8000
```

Abra seu navegador em: **`http://localhost:8000`** e clique em **"⚡ Acessar Demo (1-Clique)"**.
Para rodar os testes:
```powershell
pytest -v --cov=app tests/
```
