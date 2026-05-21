# Who's That Pokemon

Webapp om je eigen "Who's That Pokemon" te maken: upload een afbeelding, laat automatisch een silhouette/cutout genereren, en reveal daarna de originele afbeelding met je eigen naam.

## Stack

- Frontend: React + TypeScript + Vite
- Backend: FastAPI
- Image processing: Pillow + OpenCV
- Opslag: lokale SQLite + bestanden in `data/`

## Lokaal starten (zonder Docker)

1) Backend:

```bash
cd backend
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
uvicorn app.main:app --reload
```

2) Frontend (nieuwe terminal):

```bash
cd frontend
npm install
npm run dev
```

3) Open:

- Frontend: [http://localhost:5173](http://localhost:5173)
- API docs: [http://localhost:8000/docs](http://localhost:8000/docs)

## Met Docker Compose

```bash
docker compose up
```

## Testen

- Backend:

```bash
cd backend
pytest
```

- Frontend:

```bash
cd frontend
npm test
```
