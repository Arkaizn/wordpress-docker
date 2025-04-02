# WordPress Docker Setup

Dieses Repository bietet eine einfache Möglichkeit, eine WordPress-Installation mit Docker bereitzustellen. Die Konfiguration umfasst WordPress, eine MySQL-Datenbank und phpMyAdmin, alles orchestriert mit Docker Compose.

## Voraussetzungen
- Docker
- Docker Compose

## Installation
1. Klone dieses Repository:
   ```sh
   git clone https://github.com/Arkaizn/wordpress-docker.git
   cd wordpress-docker
   ```
2. Starte die Container:
   ```sh
   docker-compose up -d
   ```
3. Öffne im Browser:
   - WordPress: [http://localhost:8080](http://localhost:8080)
   - phpMyAdmin: [http://localhost:8081](http://localhost:8081)

## Konfiguration
Die Konfiguration erfolgt über die `docker-compose.yml` Datei:
- WordPress läuft auf Port `8080`
- MySQL speichert Daten in `./db_data`
- phpMyAdmin ist unter Port `8081` erreichbar

Um Umgebungsvariablen anzupassen, editiere die Datei `.env`.

## Datenbank-Zugangsdaten (Standard)
- Datenbank: `wordpress`
- Benutzer: `wp_user`
- Passwort: `wp_password`
- Host: `db`

## Nützliche Befehle
Container stoppen:
```sh
docker-compose down
```
Logs anzeigen:
```sh
docker-compose logs -f
```

## Lizenz
Dieses Projekt steht unter der MIT-Lizenz.

