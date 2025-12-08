# Visit Butuan — Local Development

Quick steps to run the site locally on Windows PowerShell.

## Prerequisites
- Python 3 installed (a virtual environment is already configured by VS Code).

## Run a Local Server
From the project root `butuantouristspots`, start a simple HTTP server:

```powershell
Push-Location "C:\Users\Mark\Documents\Projects\butuantouristspots"
C:/Users/Mark/Documents/Projects/butuantouristspots/.venv/Scripts/python.exe -m http.server 5500
```

Then open:

- http://localhost:5500/

## Notes
- Google Maps requires internet access and uses the `initMap` callback in `index.html`.
- The PHP form (`forms/contact.php`) needs a PHP-capable server to function; the Python static server won’t execute PHP. Deploy to a host with PHP or run a local PHP server for that feature.
- Static assets live under `assets/` and vendor libraries are prebundled.
