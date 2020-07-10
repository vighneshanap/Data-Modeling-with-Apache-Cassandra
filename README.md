# Data Modeling with Apache Cassandra
# Part I. ETL Pipeline for Pre-Processing the Files

# Part II. Apache Cassandra coding.
Check out the CSV file titled <font color=red>event_datafile_new.csv</font>, located within the Workspace directory to work. The event_datafile_new.csv contains the following columns:
artist
firstName of user
gender of user
item number in session
last name of user
length of the song
level (paid or free song)
location of the user
sessionId
song title
userId

# Now we need to create tables to run the following queries. Remember, with Apache Cassandra you model the database tables on the queries you want to run.
## In Apache Cassandra, you want to model your data to your queries, and if your business need calls for quickly changing requirements, you need to create a new table to process the data. That is a requirement of Apache Cassandra. If your business needs calls for ad-hoc queries, these are not a strength of Apache Cassandra. However keep in mind that it is easy to create a new table that will fit your new query.

Create queries to ask the following three questions of the data

1. Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4
2. Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182
3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

# Task 1
Query 1: Give me the artist, song title and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4

# Task 2
Query 2: Give me only the following: name of artist, song (sorted by itemInSession) and user (first and last name) for userid = 10, sessionid = 182

# Task 3
Query 3: Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

## Drop the tables before closing out the sessions
