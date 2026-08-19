# stille-zeit-web

Die beiden öffentlichen Seiten zur iOS-App **Stille Zeit**: Hilfe und
Datenschutzerklärung. Sie liegen hier, weil Apple für den App Store eine
erreichbare Support- und Datenschutz-Adresse verlangt.

Der Quellcode der App liegt **nicht** in diesem Repo, sondern privat in
`stille-zeit`.

| Datei | Zweck | App-Store-Feld |
|---|---|---|
| `index.html` | Hilfe, häufige Fragen, Anbieterangaben | Support-URL |
| `datenschutz.html` | Datenschutzerklärung | Datenschutz-URL |
| `stil.css` | gemeinsames Aussehen, Farben der App | — |

## Änderungen an der Datenschutzerklärung

Die Erklärung hat **eine** Quelle: `lib/ui/features/legal/privacy_text.dart`
im App-Repo. Von dort wird sowohl die Fassung in der App als auch
`docs/datenschutzerklaerung.md` erzeugt.

Ändert sich dort etwas, muss `datenschutz.html` hier von Hand nachgezogen
werden — sonst beschreiben App und Webseite Unterschiedliches. Der Abschnitt
zu ChurchTools erscheint in der App nur, wenn die Gemeinde-Funktion
eingeschaltet ist; im ausgelieferten Stand ist sie aus und steht deshalb
auch hier nicht.

## Veröffentlichen

GitHub Pages, Quelle `main` / Wurzelverzeichnis. Danach erreichbar unter
`https://flepsand.github.io/stille-zeit-web/`.
