# Chinook-Music-Store
A Case study on Chinook Music Store data To derive insights about popular Playlist,  Track , Album , Artist, MediaType, Genre based on customers' regionwise purchase through  Invoice, Customer, Also analyzed about Employee's performance in the store service and their service to customer based on their support to customers


Digital Music Store - Data Analysis
Data Analysis project to help Chinook Digital Music Store to help how they can optimize their business opportunities and to help answering business related questions

Find the artist who has contributed with the maximum number of albums. Display the artist name and the number of albums.

    Context: This question aims to identify the artist who has the largest body of work in terms of albums.
    Purpose: To recognize the artist who has made significant contributions to the music store's catalog.

    --1) Find the artist who has contributed with the maximum no of albums. Display the artist name and the no of albums.

SELECT name artist_name,  COUNT(albumid) no_of_albums
FROM Artist art
JOIN Album alb
ON art.artistid = alb.artistid
GROUP BY art.artistid, name
ORDER BY no_of_albums DESC



