# Weiterbildungs-Logbuch (WBO Hessen 2020)

Kostenlose, werbefreie Web-App (PWA) zur persönlichen Dokumentation der ärztlichen Weiterbildung
nach der **Weiterbildungsordnung der Landesärztekammer Hessen (WBO 2020)**.
Läuft auf **Android, iPhone/iPad und am Computer** – direkt im Browser oder als installierte App.

## Funktionen

- **Auswahldialog für die Fachrichtung**: 118 Weiterbildungsgänge der WBO Hessen
  (Facharzt-, Schwerpunkt- und Zusatz-Weiterbildungen). Nach der Auswahl passen sich Inhalte,
  Richtzahlen und Weiterbildungszeiten automatisch an. Die Fachrichtung kann jederzeit gewechselt
  oder mehrere parallel dokumentiert werden – jede Fachrichtung behält ihren eigenen Stand.
- **Tägliches Abzeichnen**: Zähler (+/−) für Richtzahlen, Haken für Kenntnisse/Fertigkeiten, Datum wählbar, Notizen.
- **Fortschritt** je Kapitel und gesamt, Verlauf aller Einträge, Suche und Filter.
- **Weiterbildungszeiten** mit Abschnitten (Abteilung, Befugte/r, Beginn, Ende, Unterbrechungen) und Anrechnung der Mindestzeiten.
- **Sicherung** als Datei (JSON), CSV-Export, druckbarer Bericht, Import einer Sicherung.
- Arbeitet **offline**, alle Daten bleiben **nur auf dem eigenen Gerät**. Es gibt keine Server, keine Konten, kein Tracking.

## Hinweise

- Bitte **keine Patientennamen oder -daten** in Notizen eintragen.
- Die Inhalte wurden automatisiert aus dem Original-PDF der WBO Hessen 2020 übernommen und stichprobenartig geprüft.
  Sie ersetzen **nicht** den Originaltext. Maßgeblich sind die aktuelle Weiterbildungsordnung und die Vorgaben der
  Landesärztekammer Hessen. **Keine Gewähr** für Vollständigkeit und Richtigkeit. Fehler bitte als Issue melden.
- Nicht enthalten: abgelaufene Bezeichnungen (z. B. Ambulante Geriatrie).
- Die App ist kein offizielles Produkt der Landesärztekammer Hessen.

## Installation für Nutzerinnen und Nutzer

Die App-Adresse (von der Person, die sie bereitstellt) im Browser öffnen:

- **Android (Chrome):** Menü (drei Punkte) → „App installieren“ bzw. „Zum Startbildschirm hinzufügen“.
- **iPhone/iPad (Safari):** Teilen-Symbol → „Zum Home-Bildschirm“. Bitte gleich am Anfang tun, bevor Daten erfasst werden:
  Die installierte iOS-App hat einen eigenen Datenspeicher, getrennt von Safari.
- **Computer:** Chrome/Edge: Installieren-Symbol in der Adressleiste.

**Sicherungen:** Daten liegen nur im Gerät. Bei Gerätewechsel, Löschen der Browserdaten oder Deinstallation sind sie weg –
daher regelmäßig unter „Daten“ → „Sicherung speichern“ (JSON). Zum Umzug dieselbe Datei dort wieder importieren.

## Veröffentlichung über GitHub Pages

Siehe `EINRICHTUNG-GITHUB.txt` im Paket. Kurz: Repository anlegen, die Dateien dieses Ordners hochladen,
unter *Settings → Pages* den Branch `main` (Ordner `/ (root)`) aktivieren.
Die App liegt dann unter `https://<benutzername>.github.io/<repository>/`.

## Dateien

| Datei | Zweck |
|---|---|
| `index.html` | die komplette App (inkl. aller Inhalte, eine einzige Datei) |
| `manifest.webmanifest` | App-Beschreibung für die Installation |
| `sw.js` | Service Worker (Offline-Betrieb) |
| `icon-*.png`, `apple-touch-icon.png` | App-Symbole |

Bei einer neuen App-Version die Zahl in `sw.js` (`logbuch-…`) und `APP_VERSION` in `index.html` erhöhen,
damit Geräte die Aktualisierung übernehmen.

Version 2.0.0 · Lizenz/Verwendung: nach Wahl der veröffentlichenden Person (z. B. MIT) – bitte eine `LICENSE`-Datei ergänzen.
