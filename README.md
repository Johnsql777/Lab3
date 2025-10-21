# CI/CD Lab — Variant №2 (Parallel jobs)

**Student number:** 2  
**Variant:** Parallel jobs — run tests and lint concurrently.

## How it works
- `test` job: runs pytest
- `lint` job: runs Black in `--check` mode

## Status badge
Replace `<YOUR-USER>` and `<YOUR-REPO>` with your GitHub details:

![CI](https://github.com/<YOUR-USER>/<YOUR-REPO>/actions/workflows/ci_variant2_parallel.yml/badge.svg)

## Local run
```bash
python -m venv .venv
. .venv/bin/activate   # Windows: .venv\Scripts\activate
python -m pip install --upgrade pip
pip install pytest black
pytest -q
black --check .
```

## Commit & push
```bash
git init
git add .
git commit -m "CI/CD Lab: Variant 2 (parallel jobs) — fixed"
git branch -M main
git remote add origin https://github.com/<YOUR-USER>/<YOUR-REPO>.git
git push -u origin main
```
