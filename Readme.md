# Calculator Demo

## Beschreibung
Dieses Projekt ist eine einfache Taschenrechner-Demo, die als Tech-Demo für Continuous Delivery dient. Es beinhaltet:
- Eine Node.js-Anwendung
- Frontend-Integration mit HTML, CSS und JavaScript
- Unit Tests mit Jest
- Containerisierung mit Docker
- Dokumentation und Checkliste für den Fortschritt

## Technologien
- **Node.js** - Serverseitige JavaScript-Laufzeitumgebung
- **Express.js** - Minimalistisches Backend-Framework für Node.js
- **Jest** - JavaScript-Testing-Framework für Unit-Tests
- **Docker** - Containerisierung für eine einheitliche Umgebung
- **GitHub Actions** - CI/CD-Tool für Automatisierung
- **ESLint** - Statische Code-Analyse für Code-Qualität


## Setup und Installation
1. Repository klonen:
   ```bash
   git clone <repository-url>
2. Abhängigkeiten installieren:
   ```bash
   npm install
3. Anwendung starten:
   ```bash
   node src/app.js
4. Tests ausführen:
   ```bash
   npm test
5. Code-Qualitätsprüfung mit ESLint:
   ```bash
   npm run lint
----------------------------------------------------------------

## Automatisierte Code-Qualitätsanalyse

### ESLint-Setup
1. Installation und konfigurieren von ESLint:
2. Code-Qualität lokal prüfen:
   ```bash
   npm run lint
3. Integration in GitHub Actions:
ESLint ist in die CI-Pipeline integriert und wird bei jedem Push automatisch ausgeführt, um die Code-Qualität zu gewährleisten.


## Containerisierung mit Docker
1. Docker-Image bauen im Root-Verzeichnis deines Projekts:
   ```bash
   docker build -t abouelfadl-techdemo .
2. Docker-Container starten:
   ```bash
      docker run -p 8080:8080 abouelfadl-techdemo
2. Anwendung testen:

Öffne einen Browser und rufe http://localhost:8080 auf, um sicherzustellen, dass die Anwendung läuft.

## Deployment auf AWS EC2
1. Docker-Image zu Docker Hub pushen

Befehl zum Einloggen in Docker Hub:
   ```bash
   docker login
   ```
   ```bash
   docker build -t alaaabou/abouelfadl-techdemo:latest .
   ```
   ```bash
   docker push alaaabou/abouelfadl-techdemo:latest
   ```

   
2. AWS EC2 Instanz starten


3. Auf AWS EC2 verbinden
   ```bash
   ssh -i <dein-key.pem> ec2-user@<EC2-PUBLIC-IP>
   ```

4. Docker installieren & Container starten

- Docker installieren 
- Docker-Image von Docker Hub ziehen
   ```bash
   docker pull alaaabou/abouelfadl-techdemo:latest
   ```
- Container starten
   ```bash
   docker run -d -p 80:3000 alaaabou/abouelfadl-techdemo:latest
   ```

- Öffne http://**[EC2-PUBLIC-IP]** im Browserum zu überprüfen

### AWS Deployment für alle sichtbar 
(nur wenn meine EC instanz läuft)

http://18.199.225.167

## Dokumentation
Siehe: [Branching-Strategie Dokumentation](docs/branching-strategy.md)

Siehe: [CI/CD-Pipeline Dokumentation](docs/cicd-pipeline.md)

## Repos für Übungen

[Exercises Repo](https://github.com/AlaaAbouElFadl/ContDelExercises)

[Workflow Automation Repo](https://github.com/AlaaAbouElFadl/contdel-uebung3)