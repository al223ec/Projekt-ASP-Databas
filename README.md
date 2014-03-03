Projekt-ASP-Databas
===================
--
<h1>
1. Problembeskrivning </h1>
<p>
Jag har tänkt göra en applikation där man kan ladda upp och visa bilder.
</p>
<p>
Användaren ska kunna ladda upp och sortera bilder till olika fotoalbum, bilder kan tillhöra många album och albumen har många tillhörande bilder.
</p>
 
●     Användare ska kunna visa bilder efter kategori.
●     Användare ska kunna visa bilder från specifika album.
●     Användare ska kunna kommentera de olika bilderna.
●     Användaren ska kunna visa alla bilder i databasen.

Avikelse
Albumpicture får en sammansatt nyckel med PictureID och AlbumID för att jag inte vill att man ska kunna lägga till samma bild flera ggr i samma album.
Placerar AlbumID först så indexeringen görs på denna nyckel i första hand. Tänker mig att man oftare behöver sortera utefter album.
Nyckeln i Comment består också den av en sammansatt nyckel PictureID först, därefter CommentID detta för att indexeringen ska göras på PictureID.
En bild måste inte finnas i Gallerypicture tabellen, dvs en bild kan finnas utan tillhörande album. Bilden kan fortfarande kommas åt från Pictures tabellen.
Bildens namn är inklusive filändelsen. 

Kommentarer
