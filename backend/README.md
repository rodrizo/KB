# backend/ — Python FastAPI (dueño: R1)

Acá va el código del backend descrito en `PROYECTO.md` (secciones 2, 3 y 4.2):

- `POST /api/transcribe`, `POST /api/agents/meeting`, `POST /api/agents/assignment`,
  `PATCH /api/tickets/{id}`, `POST /api/approve/{requirement_id}`, `GET /api/health`.
- Python 3.11+, FastAPI, Pydantic v2, OpenAI `gpt-4o-mini` (Structured Outputs), ElevenLabs Scribe.

Mientras este backend no esté corriendo, el frontend (`frontend/`) funciona igual gracias a una
simulación local fiel al contrato — ver `frontend/src/lib/api.ts` y `frontend/src/lib/mock-engine.ts`.

Para conectar el frontend a este backend real, seteá `NEXT_PUBLIC_API_URL` (ver `frontend/.env.example`).
