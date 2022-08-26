# Udacity Data Engineer Project 2: NoSQL Data Modeling 

This is the second project in the Data Engineering course. 
The assignment is outlined in the `etl.ipynb` notebook. 

The project goal was to process events from what looks to be a music streaming service. 
The log files contain data about listening sessions and which songs were played in that session.

Three queries had to be answered:

1. > Give me the artist, song title and song's length in the music app history that was heard during  sessionId = 338, and itemInSession  = 4
2. > Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
3. > Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

## Running The Project 

To run the project, a `docker-compose.yaml` file is given to start up a Cassandra database locally.
Start the database with the command `docker-compose up -d`.
Additionally, some Python dependencies should be installed.

```
python3 -m venv venv
source venv/bin/activate 
pip install -I  -r requirements.txt 
```