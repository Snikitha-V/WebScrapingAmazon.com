# WebScrape_Amazon

Small scraper to extract title and price from a single Amazon product page.

**Setup**
- **Python:**: Tested with Python 3.13+. Ensure Python is installed.
- **Virtualenv:**: Create and activate the included venv or use your own.

```powershell
C:/Python313/python.exe -m venv webScrape
.\webScrape\Scripts\Activate.ps1
.\webScrape\Scripts\python.exe -m pip install -r requirements.txt
```

**Usage**
- **Run interactively:**: Run the script and paste a product URL when prompted.

```powershell
.\webScrape\Scripts\python.exe scrape.py
```

- **Run without activating venv:**: Use the venv python directly.

```powershell
.\webScrape\Scripts\python.exe scrape.py
```

**Files**
- `scrape.py`: The scraper script that prompts for an Amazon product URL and prints title/price.
- `requirements.txt`: Python package dependencies (requests, beautifulsoup4, lxml).
- `.gitignore`: Excludes the `webScrape` venv and common artifacts.

**Notes**
- This tool is for educational purposes. Scraping Amazon may violate their Terms of Service; use responsibly.
- If PowerShell blocks activation, run: `Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass -Force` then activate.
