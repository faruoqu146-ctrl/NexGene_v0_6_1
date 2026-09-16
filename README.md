# NexGene v0.6

The first product-facing NexGene interface.

## Added
- Responsive mobile web interface
- Login and account creation
- Morning and evening check-ins
- Today's health snapshot
- Longitudinal timeline
- Personal trend insights
- Server-authenticated user identity

## Run
```bash
docker compose up --build
```
Open http://localhost:8000

API docs: http://localhost:8000/docs

## Test
```bash
docker compose exec api pytest -q
```

This is still a private development prototype. Do not enter real patient, clinical, genetic, or production credentials.
