# TrafficCongestionModel
The data file for manuscript of Processes and Events in the Centre: A taxi trajectory-based approach to detect traffic congestion and analyse causes
#############

Method 1: Use our database file
Three steps to quickly improt the experiment data.
  Step 1: unzip the Neo4j.zip file and import it into the Neo4j database. The unzipped Neo4j file is a database backup file that can be directly hooked up by modifying     the database name in conf.
  Step 2: After importing to Neo4j database, you can check "The profile of the database in neo4j.docx" to see if the database is imported correctly, and implement the      query according to the word file.
  Step 3: The application and reasoning of the model is detailed in the query reasoning statements provided in the paper, and the database model system provides fast       retrieval and querying.
#####################
Method 2: Use the batch modeling results CSV file to import the results library.
  Step 1: Download csv files.
  Step 2: copy the import sentence as bellow into neo4j-admin import window:
      neo4j-admin import --database=neo4j --nodes=import/State.csv --nodes=import/Process.csv --nodes=import/Grid.csv --relationships=import/Contain.csv --relationships=import/Next.csv --relationships=import/Precede.csv --relationships=import/Include.csv --skip-duplicate-nodes=true --skip-bad-relationships=true --ignore-extra-columns=true
  Step 3: After importing to Neo4j database, you can check "The profile of the database in neo4j.docx" to see if the database is imported correctly, and implement the      query according to the word file.
  Step 4: The application and reasoning of the model is detailed in the query reasoning statements provided in the paper, and the database model system provides fast       retrieval and querying
