## Checkliste für die eigene fortlaufende Übung / TechDemo in Continuous Delivery

### Einführung und Grundlagen
- [x] Verständnis von Continuous Delivery und dessen Bedeutung
- [x] Unterschiede zwischen Continuous Integration, Continuous Delivery und Continuous Deployment
- [x] CI-Anti Pattern identifizieren

### 20% Projekt Setup
- [x] Initialisierung des Repository (Git) -> (Blank Project + Project Name = nachname) 
- [x] Checkliste kopieren und in neues geklontes Repository/project einfügen
- [x] Checkliste versionieren
- [x] README anfertigen mit Verlinkungen, Hinweisen, etc. zum Inhalt des Repository
- [x] zweites Repository für Übungen, Ausprobieren, etc. inkl. README sowie Verlinkungen und Übersicht zu den Übungen
- [x] .gitignore angepasst: Stelle sicher, dass unnötige Dateien nicht im Repository landen (z. B. durch ein angepasstes .gitignore-File).

### 10% Automatisierung
- [x] Automatisierte Builds eingerichtet
- [x] Automatisierte Tests implementiert
- [X] Automatisierte Deployments konfiguriert
- [x] Automatisierte Code-Qualitätsanalyse: Setze statische Code-Analyse-Tools ein, um Codequalität automatisiert zu überprüfen.

### 10% Testing
- [x] (Unit) Tests geschrieben und automatisiert
- [ ] Integrationstests implementiert (optional)
- [ ] End-to-End Tests eingerichtet (optional)

### Deployment-Strategien
- [X] Deployment-Strategien identifizieren
- [X] Rollback-Strategien (optional)

### 10% Containerisierung
- [x] Docker oder ähnliche Technologien eingesetzt
- [x] Integration in eine Build-Pipeline

### 20% Infrastruktur- und Konfigurationsmanagement
- [X] Template Konfigurationsdateien versioniert und zentralisiert
- [X] Konfigurationsdateien ausgenommen
- [X] Verwendung in einer Build-Pipeline
- [ ] Infrastructure as Code (IaC): Nutze Tools wie Terraform oder Ansible, um die Infrastruktur als Code zu verwalten und sicherzustellen, dass Deployments wiederholbar sind.

### 10% Sicherheit
- [X] Zugangsdaten sicher hinterlegt
- [ ] Sicherheitsüberprüfungen: Integriere automatisierte Sicherheitstests (z. B. OWASP ZAP) in die Pipeline, um potenzielle Sicherheitslücken frühzeitig zu erkennen.

### Datenbanken
- [ ] Datenbank-Migrationen automatisiert
- [ ] Datenbank-Backups und Recovery-Pläne

### 20% Abschluss und Dokumentation
- [X] Projekt-Dokumentation vervollständigt
- [X] Branching-Strategie dokumentieren: Definiere eine Branching-Strategie (z. B. GitFlow) und dokumentiere die Entscheidungsfindung.
- [X] Pipeline-Dokumentation: Erstelle eine vollständige technische Dokumentation deiner CI/CD-Pipeline, einschließlich aller verwendeten Tools, Skripte und Konfigurationen.
- [X] Build Pipeline spezifizieren: Stelle sicher, dass alle Schritte der CI/CD-Pipeline klar definiert sind, inklusive Test-, Build- und Deployment-Schritte.
