# Project Evolution

## swyby-ai-engine

### 2026-05 — Project Launch

The `swyby-ai-engine` repository was created as the public-facing AI engine for Swyby.

**Key architectural decisions:**
- Python 3.12 + asyncio for high-concurrency signal processing
- PostgreSQL for reliable data persistence
- WebSocket layer for real-time communication
- Environment-based configuration for deployment flexibility

**Design goals:**
- Clean separation between signal processing and recommendation logic
- Walk-forward validation for recommendation quality
- Gapless data handover for zero-downtime updates
- Multi-strategy portfolio selection based on context

**Relationship to Swyby ecosystem:**
This engine powers the activity recommendations in the Swyby mobile app and dashboard.
It connects to the event aggregator (`koh_phangan_events`) for data input and serves
recommendations through the backend API (`phangan_api`).

---

*Note: This project builds upon 20+ years of engineering experience, including earlier*
*work in signal processing and real-time systems. The current architecture represents*
*a clean redesign focused specifically on activity recommendation use cases.*
