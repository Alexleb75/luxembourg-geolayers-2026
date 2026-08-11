# luxembourg-geolayers-2026

Couches GeoJSON du Luxembourg pour **GEOlayers 3** (After Effects), organisées par géographie.

**Utilisation** : dans GeoLayers → Feature Search → source **GitHub Repo** → URL nue de ce repo, branche `main`.
La recherche se fait **par nom de fichier** ; le chemin du dossier s'affiche comme contexte.

## Structure (1 fichier = 1 entité)
```
District <D>/
  District <D>.geojson
  Canton <C>/
    Canton <C>.geojson
    <Commune>/
      <Commune>.geojson
      Parcs/       <parc>.geojson        (ex. Kinnekswiss)
      Quartiers/   <quartier>.geojson    (délimitation OSM, sinon point)
      Lieux-dits/  <lieu-dit>.geojson
      Monuments/   <monument>.geojson
```
Districts historiques (supprimés en 2015, gardés comme niveau racine) : Luxembourg, Diekirch, Grevenmacher.

## Agrégats (racine) — pour charger une couche entière d'un coup
`luxembourg-communes/-cantons/-districts/-parcs/-quartiers/-lieux-dits/-monuments.geojson`

## Sources
Communes/cantons : [click_that_hood](https://github.com/codeforgermany/click_that_hood).
Parcs, quartiers, lieux-dits, monuments : OpenStreetMap. Propriété de nom : `name`.
