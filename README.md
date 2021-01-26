# Exo sur Monet

# liste des peintures de Claude Monet

select DISTINCT ?peinture 
where {
 ?peinture wdt:P170 wd:Q296.
 }
 
# Avec les labels (via le service wikibase:label) et les images associées

#Tableaux de Claude Monet
#defaultView:ImageGrid
SELECT *
WHERE
{
  ?item wdt:P31 wd:Q3305213 .
  ?item wdt:P170 wd:Q296.
  ?item wdt:P18 ?pic .
}
# # avec en option (via OPTIONAL) les collections/lieux de
conservation
#Lieux ou se trouvent les œuvres de Claude Monet
#defaultView:Map
SELECT ?label ?coord ?subj
WHERE
{
   ?subj wdt:P170 wd:Q296.
  OPTIONAL {?subj wdt:P276 ?loc .
    ?loc wdt:P625 ?coord } .   
   ?subj rdfs:label ?label filter (lang(?label) = "fr")
}
# LES GRANDES FAMILLES DE FROMAGES
![alt tag](https://4.bp.blogspot.com/-IQPaUaAZW5g/WHaeD_2PB_I/AAAAAAAAGHg/_ljyMGR5YRwMYqT3T8_21aj4SY-6ICPGwCLcB/s1600/fromages.jpeg)
### les données utilisées proviennent de la "Liste des Fromages Français"
<iframe src="https://data.opendatasoft.com/explore/embed/dataset/fromagescsv-fromagescsv@public/table/?disjunctive.fromage&sort=departement&dataChart=eyJxdWVyaWVzIjpbeyJjb25maWciOnsiZGF0YXNldCI6ImZyb21hZ2VzY3N2LWZyb21hZ2VzY3N2QHB1YmxpYyIsIm9wdGlvbnMiOnsiZGlzanVuY3RpdmUuZnJvbWFnZSI6dHJ1ZSwic29ydCI6ImRlcGFydGVtZW50IiwibG9jYXRpb24iOiI1LDQ2LjY2NjE5LDIuOTEyMDgiLCJiYXNlbWFwIjoiamF3Zy5zdHJlZXRzIn19LCJjaGFydHMiOlt7ImFsaWduTW9udGgiOnRydWUsInR5cGUiOiJib3hwbG90IiwiZnVuYyI6IkNPVU5UIiwic2NpZW50aWZpY0Rpc3BsYXkiOnRydWUsImNvbG9yIjoicmFuZ2UtY3VzdG9tIiwiY2hhcnRzIjpbeyJmdW5jIjoiTUlOIn0seyJmdW5jIjoiUVVBTlRJTEVTIiwic3Vic2V0cyI6MjV9LHsiZnVuYyI6IlFVQU5USUxFUyIsInN1YnNldHMiOjUwfSx7ImZ1bmMiOiJRVUFOVElMRVMiLCJzdWJzZXRzIjo3NX0seyJmdW5jIjoiTUFYIn1dfSx7ImFsaWduTW9udGgiOnRydWUsInR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQ09VTlQiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiJyYW5nZS1jdXN0b20ifV0sInhBeGlzIjoiZGVwYXJ0ZW1lbnQiLCJtYXhwb2ludHMiOjUwLCJzb3J0IjoiIiwic2VyaWVzQnJlYWtkb3duIjoibGFpdCIsInNlcmllc0JyZWFrZG93blRpbWVzY2FsZSI6IiJ9XSwidGltZXNjYWxlIjoiIiwiZGlzcGxheUxlZ2VuZCI6dHJ1ZSwiYWxpZ25Nb250aCI6dHJ1ZSwic2luZ2xlQXhpcyI6dHJ1ZX0%3D&location=5,46.66619,2.91208&basemap=jawg.streets&static=false&datasetcard=true" width="850" height="400" frameborder="0"></iframe>
### L’utilisation du lait cru dans la production des frommages selon les departements
<iframe src="https://data.opendatasoft.com/explore/embed/dataset/fromagescsv-fromagescsv@public/analyze/?disjunctive.fromage&sort=departement&dataChart=eyJxdWVyaWVzIjpbeyJjb25maWciOnsiZGF0YXNldCI6ImZyb21hZ2VzY3N2LWZyb21hZ2VzY3N2QHB1YmxpYyIsIm9wdGlvbnMiOnsiZGlzanVuY3RpdmUuZnJvbWFnZSI6dHJ1ZSwic29ydCI6ImRlcGFydGVtZW50IiwibG9jYXRpb24iOiI1LDQ2LjY2NjE5LDIuOTEyMDgiLCJiYXNlbWFwIjoiamF3Zy5zdHJlZXRzIn19LCJjaGFydHMiOlt7ImFsaWduTW9udGgiOnRydWUsInR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQ09VTlQiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiJyYW5nZS1jdXN0b20ifSx7ImFsaWduTW9udGgiOnRydWUsInR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQ09VTlQiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiJyYW5nZS1jdXN0b20ifSx7ImFsaWduTW9udGgiOnRydWUsInR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQ09OU1RBTlQiLCJzY2llbnRpZmljRGlzcGxheSI6dHJ1ZSwiY29sb3IiOiJyYW5nZS1jdXN0b20iLCJ5QXhpcyI6MH0seyJhbGlnbk1vbnRoIjp0cnVlLCJ0eXBlIjoiY29sdW1uIiwiZnVuYyI6IkNPVU5UIiwic2NpZW50aWZpY0Rpc3BsYXkiOnRydWUsImNvbG9yIjoicmFuZ2UtY3VzdG9tIn1dLCJ4QXhpcyI6ImRlcGFydGVtZW50IiwibWF4cG9pbnRzIjoyMDAsInNvcnQiOiIiLCJzZXJpZXNCcmVha2Rvd24iOiJsYWl0Iiwic3RhY2tlZCI6IiIsInNlcmllc0JyZWFrZG93blRpbWVzY2FsZSI6IiJ9XSwidGltZXNjYWxlIjoiIiwiZGlzcGxheUxlZ2VuZCI6dHJ1ZSwiYWxpZ25Nb250aCI6dHJ1ZSwic2luZ2xlQXhpcyI6dHJ1ZX0%3D&location=5,46.66619,2.91208&basemap=jawg.streets&static=false&datasetcard=false" width="880" height="650" frameborder="0"></iframe>

Les fromages sont essentiellement fabriqués grâce au lait de vache, de chèvre et de brebis.
Le lait de vache, qui est majoritairement utilisé, est présent dans presque tous les départements français sauf dans trois départements, à savoir Hérault, Indre et Ille-et-Vilaine. Ces trois départements utilisent exclusivement le lait de chèvre qui est le deuxième type de lait le plus utilisé derrière le lait de vache.
Le lait de brebis, qui arrive en troisième position de ce classement est aussi utilisé majoritairement dans certains départements tels que Aveyron, Hautes-Pyrénées… et même exclusivement dans un seul département tel que la Haute-Corse


### Repartition par départements avec les liens wikipédia

Liste des spécialités régionales françaises de fromages. la selection d'un departement au choix, sur la carte, permet d'avoir la page wikipédia du produit.

<iframe frameborder="0" width="900" height="650" src="https://fromage.trial.opendatasoft.com/map/embed/fromage_fr/?&static=false&scrollWheelZoom=false"></iframe>
# Présentation du Top 5 des fromages préférés des français.
<iframe width="900" height="400" src="https://www.youtube.com/embed/pOZ1DXy0mlE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen ></iframe>
