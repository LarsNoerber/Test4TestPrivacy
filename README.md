# Test4Test – Datenschutzhinweise

Öffentliche Seite: https://larsnoerber.github.io/Test4TestPrivacy/

GitHub Pages veröffentlicht `index.html` aus `main`, Verzeichnis `/`. Die Seite ist statisch;
sie enthält keine Analysewerkzeuge, externen Schriftarten oder App-Sitzungstoken.

Der Kontolöschungsweg ist direkt verlinkt: https://test4test.noerber.de/delete-account/

Die Hinweise bilden die aktuelle App ab: Google-Anmeldung, Testbeitritte und UTC-Check-ins,
Apps der Tester, lokale Paketprüfung, direkte Icon-Abrufe und Bildcache sowie Kontolöschung.
Febas stellt Domain, Webspace, API und Datenbank bereit. GitHub Pages hostet nur diese Seite.

Name und E-Mail-Adresse des Verantwortlichen sind veröffentlicht. Die Postanschrift wird auf
Wunsch des Betreibers später ergänzt. Konkrete Hosting-Log- und Backup-Fristen sowie die
vertragliche Auftragsverarbeitung werden nicht aus allgemeinen Anbieter-Webseiten erfunden.

Geprüfte Anbieterquellen, Stand 15. November 2026:

- https://www.febas.de/datenschutz/
- https://www.febas.de/agb.php
- https://www.febas.de/impressum/
- https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages#data-collection
- https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement

App-Quellen: https://github.com/LarsNoerber/Test4Test

## Gemeinsame Quelle und Aktualisierung

`policy.json` ist die einzige JSON-Quelle für Deutsch und Englisch. Im Elternprojekt
erzeugt `python scripts/render-privacy.py` daraus die Abschnitte in `index.html` und
die Web-Offline-Kopie `web-client/public/policy.json`. `--check` prüft beide Kopien.
Die HTML-Seite enthält beide Sprachen mit direkten Sprachlinks. Die native Android-App
übernimmt die Quelle über den Gradle-Task `:app:prepareOfflinePrivacy` und lädt zur
Laufzeit weiterhin die veröffentlichte JSON-Datei mit lokalem Offline-Fallback.

Stand 21.11.2026 ergänzt: ausgewählte Bilddateien ohne allgemeine Galerie-Berechtigung,
automatischer Upload nach Auswahl, Metadaten/privater Bildspeicher, Bildmeldungen und
Löschwege, optionale Gerätesperre, Browser-Speicher und technische Missbrauchszähler.
Noch unbestätigte Betreiber-/Hostingangaben werden nicht von anderen Webseiten übernommen.
