# malaria-neo4j
Project to build a neo4j instance with some data sets for Malaria (P. falciparum)
Before running any cypher script, please update it with your local project location

* Install and start neo4j
* Create the nodes running createNodes.cypher using the neo4j shell:
   {neo4j dir}/bin/neo4j-shell -file createNodes.cypher > import.txt
* Add multi labels on the nodes running addMultiLables.cypher:
   {neo4j dir}/bin/neo4j-shell -file addMultiLabels.cypher
* Create the indexes
   {neo4j dir}/bin/neo4j-shell -file createIndexes.cypher
* Create some relationships (genes and organisms, genes and proteins, datasets and datasources, ontology and ontology terms, gene      and go annotation, overlaps):
   {neo4j dir}/bin/neo4j-shell -file createRelationships1.cypher
   {neo4j dir}/bin/neo4j-shell -file createRelationships3.cypher
