# M347
**Verzeichnis erstellen** <br>
mkdir webserver <br>
cd webserver<br>
mkdir website<br>

**Index Datei hinzufügen**<br>
touch index.html<br>

**Dockerfile erstellen**<br>
touch Dockerfile<br>

**Image bauen**<br>
docker build -t webserver .<br>

**Container starten**<br>
docker run -p 8080:80 -v $(pwd)/webseite:/usr/local/apache2/htdocs/ -v
$(pwd)/logs:/usr/local/apache2/logs/ webserver
