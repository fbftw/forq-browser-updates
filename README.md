# FORQ Browser – Setup und Updates

Dieses Repository enthält **nur die veröffentlichten Dateien** von FORQ Browser, keinen Quellcode.

- **Erstinstallation:** `FORQ-Browser-Setup.exe` aus dem [neuesten Release](https://github.com/fbftw/forq-browser-updates/releases/latest) herunterladen und ausführen. Es sind keine Administratorrechte nötig.
- **Updates:** Ab Fassung 0.8.0 fragt FORQ Browser hier selbst nach einer neueren Fassung und bietet sie an. Ersetzt wird erst nach Ihrer Zustimmung.

Die erste Fassung, die über dieses Repository verteilt wird, ist 0.8.0. Wer eine ältere Fassung installiert hat, installiert 0.8.0 einmal mit dem Setup; danach kommen Updates von selbst.

## Dateien je Release

| Datei | Zweck |
|---|---|
| `FORQ-Browser-Setup.exe` | Installation bzw. manuelles Update |
| `freigabe.json` | signierte Freigabe (Fassung, Prüfsumme des Pakets) |
| `FORQ-Browser-<Fassung>.forqcomponent` | Update-Paket für die automatische Aktualisierung |
| `*.sha256` | Prüfsummen |

FORQ Browser nimmt ein Update nur an, wenn `freigabe.json` mit dem Freigabeschlüssel der FORQ-Familie signiert ist und das Paket genau zur signierten Prüfsumme passt. Eine veränderte oder untergeschobene Datei wird abgelehnt.
