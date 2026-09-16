# Test report: NexGene_v0_6_1.zip

Date: 2026-09-16

## Archive tests

| Check | Result |
| --- | --- |
| Zip exists | Pass (707 bytes) |
| `unzip -t` integrity | Pass — no errors |
| Contents | `NexGene_v0_6_1/` directory + `README.md` only |
| Extract | Pass |
| README size | 565 bytes |
| SHA-256 zip | `c5fd70a338e6f1fb127f23dad92fd038fd1f223a1da12cdbde314fa832b26ee6` |
| SHA-256 README | `607eb28a86a73fded311c03bd8eaee4e85aff1c3322095e8953d79e88d32911d` |
| Secrets in README | None found |

## Application tests (blocked)

The zip does **not** contain application source.

Missing files required by the README:
- `docker-compose.yml`
- `Dockerfile` / backend / mobile
- `pytest` suite
- API server for `localhost:8000` and `/docs`

Therefore these could **not** be run:
- `docker compose up --build`
- `docker compose exec api pytest -q`
- HTTP/API/auth/check-in/timeline/insights UI tests
- Mobile responsiveness tests

## Comparison

A full tree already exists on GitHub at [faruoqu146-ctrl/NexGene_v0_6](https://github.com/faruoqu146-ctrl/NexGene_v0_6) (Docker, backend, mobile, tests). This `v0_6_1` zip is a README-only snapshot, not a runnable increment.

## Verdict

Archive is valid but incomplete. Product features listed in the README cannot be tested from this zip alone.
