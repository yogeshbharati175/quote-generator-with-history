# Quote Generator with History (Python)
Beginner-friendly Flask project with quote API integration, local fallback quotes, copy-to-clipboard, and SQLite favorites history.

## Run in Windows PowerShell
```powershell
python -m venv venv
.\\venv\\Scripts\\Activate.ps1
python -m pip install -r requirements.txt
python app.py
```
Open http://127.0.0.1:5000

If activation is blocked:
```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
.\\venv\\Scripts\\Activate.ps1
```

## API
- `GET /api/quote` get a random quote
- `GET /api/favorites` list saved quotes
- `POST /api/favorites` save quote JSON: `{"quote":"Text","author":"Name"}`
- `DELETE /api/favorites/<id>` remove saved quote

SQLite database is created automatically.
