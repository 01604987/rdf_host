# rdf_host
This public repository will serve as a makeshift solution for publicly hosting rdf files, in specific ttl and json-ld.

Upload the desired rdf into their folders and access them publicly via their github pages url.<br>
The resolved links will be automatically matched to the files corresponding content type, allowing parsing and fetching rdfs.

Example using rdflib:
```
from rdflib import Graph

g = Graph()

g.parse('https://01604987.github.io/rdf_host/rdf/machinedata.ttl')
    
print(g.serialize(format="json-ld"))
```
