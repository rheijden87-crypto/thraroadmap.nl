# Beveiligingsnotities

## Publieke client
Deze GitHub Pages-site draait volledig in de browser. Alle waarden in `index.html`, inclusief de Supabase-URL en publishable key, zijn zichtbaar voor bezoekers.

## Vereist in Supabase
- Schakel Row Level Security in op `thra_roadmap` en `thra_wensen`.
- Geef anonieme bezoekers alleen de handelingen die werkelijk openbaar mogen zijn.
- Overweeg alleen-lezen toegang voor de roadmap en beperkte `INSERT`-toegang voor wensen.
- Beperk `UPDATE` en `DELETE` bij voorkeur tot aangemelde beheerders.
- Plaats nooit een Supabase service-role key in deze repository of in browsercode.

## Voor ingebruikname
Controleer in een privévenster wat een niet-aangemelde bezoeker kan lezen en wijzigen.
