# THRA Ontwikkelingsroadmap

Interactieve roadmap voor moduleontwikkeling, gemaakt als zelfstandige HTML/CSS/JavaScript-app en gekoppeld aan Supabase.

## Bestanden

- `index.html`: de website
- `404.html`: fallback voor GitHub Pages
- `.nojekyll`: voorkomt verwerking door Jekyll
- `CNAME`: koppelt de site aan `thraroadmap.nl`
- `robots.txt`: instructies voor zoekmachines
- `sitemap.xml`: sitemap voor het hoofddomein
- `.gitignore`: sluit lokale systeembestanden uit

## Publiceren via GitHub Pages

1. Upload alle bestanden uit deze map naar de hoofdmap van de repository.
2. Open in GitHub: **Settings > Pages**.
3. Kies bij **Build and deployment** voor **Deploy from a branch**.
4. Selecteer branch **main** en map **/(root)**.
5. Sla de instelling op.
6. Koppel bij de domeinprovider de DNS-records aan GitHub Pages.
7. Activeer in GitHub Pages **Enforce HTTPS** zodra dit beschikbaar is.

## Supabase

De website gebruikt een publieke Supabase publishable key in de browser. Zorg dat Row Level Security en policies voor de tabellen `thra_roadmap` en `thra_wensen` bewust zijn ingericht. Zonder beperkende policies kunnen publieke bezoekers mogelijk gegevens toevoegen, wijzigen of verwijderen.

## Lokaal testen

Open `index.html` rechtstreeks in een browser. Voor een test via een lokale webserver kan bijvoorbeeld VS Code Live Server worden gebruikt.
