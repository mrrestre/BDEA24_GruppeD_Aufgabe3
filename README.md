# BDEA24_GruppeD_Aufgabe3

# Aufgabe Beschreibung

- Mindestens eine NoSQL DB verwenden (Docker, Docker-compose)
- Lessons Learned wichtiger als optimale Lösung (Was hätte ich anders gemacht?)

1. Abzugeben:
- Dockerfile / Dockercompose pro DB
- PDF Datenmodell -> Aufbau von System
- Skript / Programm zum Laden von Daten in die DB
- Abfragen zum Szenarien
- PDF Lessons Learned (`lessons-learned.pdf`)

2. DB:
- Sollte auf mehrere Container / Knoten laufen
  - Wenn es nicht geht, erklären wieso das nicht ging / was dafür gebraucht ist

3. App
- Laden von Init-Daten
- Abfragen feuern
- Inhalt anzeigen

4. Systemanforderungen
- Es gibt:
  - Follower-Beziehungen
  - Posts von Prominenten
- Aufgaben:
  - Posts von Prominenten auf die 100 IDs verteilen, die am meisten Follower haben (Influencer)
  - Posts können geliked werden (von welchem User wurde ein Post eines anderen Users geliked)
    - Zufällig generiert
- Anfragen:
  - Auflistung von zu einem Account zugeordneten Posts
  - Auflistung der 100 Accounts mit den meisten Followern (Influencer)
  - Auflistung der 100 Accounts, die den meisten Influencer folgen
  - Startseite für ein beliebiges Account (Influencer sind hier gut):
    - Anzahl Followers
    - Anzahl gefolgte Accounts
    - 25 Posts von gefolgten Accounts:
      - Neueste
      - Meisten Likes
    - Caching der Posts für die Startseite
    - Auflistung der 25 Posts, die ein Wort beinhalten:
      - (Optional: Und-verknüpfte Wörter)
