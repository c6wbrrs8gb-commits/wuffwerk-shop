# Hütepfote – Anweisungen für Codex und Agenten

## Projektziel

Hütepfote ist ein deutscher Onlineshop für hochwertiges Hundezubehör. Das Projekt soll einfach wartbar, schnell, mobilfreundlich, hochwertig gestaltet, für GitHub Pages geeignet und möglichst kostengünstig bleiben. Als Geschäftsmodell ist Direktversand statt Lagerhaltung vorgesehen.

## Projektarchiv und Technik

- Projektarchiv: `OrdinaryOnonas/wuffwerk-shop`
- Standard-Branch: `main`
- Die Website ist eine statische GitHub-Pages-Website.
- Bevorzugt werden HTML5, CSS3 und reines JavaScript.

Keinen Server, keine Datenbank, kein Build-System, kein Framework und keinen kostenpflichtigen Dienst ohne ausdrückliche Anforderung hinzufügen. React, Vue, Next.js, Node-Build-Werkzeuge, Tailwind und Bootstrap nur nach ausdrücklicher Freigabe verwenden. `index.html` muss ohne zusätzliche Werkzeuge nutzbar bleiben.

## Gestaltung und Tonalität

Hütepfote soll klar, modern und hochwertig wirken, mit großzügigen Freiräumen, deutlicher Typografie, abgerundeten Karten, dezenten Schatten, zurückhaltenden Farben, großen Produktbildern und leichten Animationen. Die Marke bleibt **Hütepfote**; die Ansprache ist modern, vertrauenswürdig, freundlich, hochwertig und hundebezogen. Die Website darf nicht wie eine beliebige Vorlage oder ein Marktplatz wirken.

## Produkte und Bilder

Produkte benötigen deutsche Namen, kurze nutzenorientierte Beschreibungen, realistische Preise, hochwertige Bilder, klare Schaltflächen und mobilfreundliche Darstellung. Niemals Lieferantenpreise, Lieferzeiten, Bewertungen, Zertifikate, Spezifikationen, Garantien oder Lagerbestände erfinden. Unbekannte Angaben konfigurierbar lassen oder klar als zu prüfen kennzeichnen.

Realistische Produktfotografie verwenden; keine offensichtlich künstlichen Platzhalterbilder im fertigen Shop. KI-Bilder müssen realistisch sein, zur Marke passen und dürfen weder ein konkretes Lieferantenprodukt vortäuschen noch gefälschte Kundenbewertungen erzeugen.

## Warenkorb und Bestellung

Der Warenkorb muss Produkte hinzufügen, Mengen ändern und Produkte entfernen können, Zwischensumme und Gesamtsumme zeigen, mobil funktionieren und bei Bedarf lokal im Browser gespeichert werden. Für den statischen Warenkorb `localStorage` nutzen, aber niemals sensible Zahlungsdaten dort speichern.

Der aktuelle Bestellablauf ist nur eine Demonstration. Bis ein echter Zahlungs- und Serverdienst ausdrücklich beauftragt ist, keine Zahlung oder echte Bestellung behaupten, keine Kundendaten an Dritte übermitteln und keine Zahlungsdaten speichern. Für eine echte Bestellung einen geeigneten Zahlungsanbieter und eine serverseitige Verarbeitung einsetzen. Niemals Kreditkartendaten direkt im JavaScript der Website verarbeiten.

## Rechtliches und Datenschutz

Impressum, Datenschutz, Widerruf und AGB sind Platzhalter, bis die tatsächlichen Unternehmens- und Rechtsdaten vorliegen. Niemals Firmendaten, Anschriften, Umsatzsteuer-IDs, Registernummern oder Rechtsbehauptungen erfinden. Vor dem Verkaufsstart klar auf die notwendige Finalisierung der Rechtstexte hinweisen.

Nie API-Schlüssel, Passwörter oder andere Geheimnisse im Projekt speichern, private Zugangsdaten veröffentlichen oder Kundendaten an unbekannte Dienste schicken. Falls ein Geheimnis erforderlich ist, zuerst eine sichere Architektur erklären statt es in `index.html` einzufügen.

## Direktversand und Kosten

Lieferanten aus Deutschland oder der EU bevorzugen. Auf kurze Lieferzeiten nach Deutschland, verlässliche Lieferanten, transparente Produktdaten, angemessene Versandkosten, gute Bewertungen, geringes Retourenrisiko und ausreichende Marge achten. Produkte nicht nur wegen eines günstigen Einkaufspreises veröffentlichen.

Immer berücksichtigen:

`Verkaufspreis - Produktkosten - Versand - Zahlungsgebühren - erwartete Retouren - Steuern = realistischer Deckungsbeitrag`

Eine geschätzte Marge niemals als garantierten Gewinn darstellen. Die derzeitige Produktausrichtung umfasst Schnüffelmatten, Reise-Trinkflaschen, Beschäftigungsspielzeug, LED-Halsbänder und -Leinen sowie Autoschutzdecken. Händlerpreise von ZooDrop / Pet-Star erst nach Händlerregistrierung verwenden.

## Qualität, Barrierefreiheit und Änderungen

Code lesbar, gut strukturiert, angemessen kommentiert, barrierearm, responsiv und schlank halten. Funktionierende Abläufe bei Änderungen erhalten, unnötige Duplikate vermeiden und das vorhandene Verhalten vor einem Austausch verstehen.

Semantisches HTML, Beschriftungen für Formularfelder, tastaturbedienbare Elemente, aussagekräftige Alternativtexte, ausreichende Kontraste und sichtbare Fokuszustände verwenden. Wichtige Informationen nie ausschließlich über Farbe vermitteln.

Bei jeder Änderung:

1. Vorhandenen Code prüfen.
2. Funktionierende Abläufe bewahren.
3. Die kleinste sinnvolle Änderung vornehmen.
4. Betroffene Funktionen testen.
5. Desktop- und Mobilansicht prüfen.
6. Änderungen erklären.

Die gesamte Website nicht ohne Not neu schreiben.

## Git und GitHub

Klare Commit-Nachrichten verwenden, kleine verständliche Commits bevorzugen und niemals ohne ausdrückliche Anweisung einen erzwungenen Push oder eine Überschreibung der Historie durchführen.

Codex darf auf Wunsch Projektstand und GitHub verwalten, einschließlich Branches, Commits, Pushes, Pull Requests und Issues. Vor irreversiblen oder weitreichenden Schritten – etwa dem Löschen von Remote-Branches oder Dateien, einem erzwungenen Push, dem Zusammenführen eines Pull Requests, Änderungen an Repository-Einstellungen oder Veröffentlichungen – Ziel exakt nennen und die ausdrückliche Freigabe des Eigentümers einholen. Nach jeder GitHub-Aktion Branch, Commit, Pull Request, Issue oder Datei mitteilen.

## Vorrangregel

Diese Datei ist die projektspezifische Grundlage für Änderungen an Hütepfote. Markenname und Kernfunktionen nicht entfernen, keine unnötigen Frameworks oder kostenpflichtigen Dienste einführen und keine Geschäfts- oder Lieferanteninformationen erfinden. Die neueste ausdrückliche Anforderung des Nutzers hat Vorrang, solange Sicherheit, Datenschutz, rechtliche Vorgaben und bestehende Funktionen gewahrt bleiben.
