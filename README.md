# KassenKompass – erster Prototyp

## Was enthalten ist
- Mehrere Kassen mit frei wählbarem Namen
- Einnahmen und Ausgaben
- Bei Ausgaben: zahlende Person und Auswahl, ob eine Erstattung offen ist
- Offene Erstattungen als bezahlt markieren
- Auslagenübersicht je Person
- JSON-Datenexport

## Lokal ausprobieren
Öffne `index.html` in einem aktuellen Browser. Für die Installation als PWA muss das Projekt über HTTPS (oder localhost) bereitgestellt werden.

## Wichtiger Entwicklungsstand
Dies ist ein funktionsfähiger UI-/Logik-Prototyp. Er speichert aktuell lokal im Browser (`localStorage`). OneDrive-Synchronisierung, persönliche Benutzerkonten, Rollen/Rechte und sichere gemeinsame Mehrbenutzer-Buchungen sind NOCH NICHT implementiert. Bitte noch keine echten Finanzdaten verwenden.

## Nächste technische Ausbaustufe
1. Microsoft Entra App-Registrierung für persönliche Microsoft-Konten und OAuth-Anmeldung.
2. Microsoft Graph-Anbindung an den freigegebenen OneDrive-Ordner.
3. Konfliktfreie Schreiblogik/Transaktionsjournal für parallele Buchungen.
4. Benutzer- und Kassenberechtigungen.
5. Beleg-Upload in OneDrive.
6. Hosting unter einer HTTPS-Adresse, damit alle die App installieren können.

Für eine robuste Mehrbenutzerlösung muss die OneDrive-Integration vor Veröffentlichung sicher getestet werden. Ein statischer Client darf keine Client-Secrets enthalten.
