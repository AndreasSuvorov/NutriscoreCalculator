# NutriScore-Rechner

Dieses Projekt ist ein NutriScore-Rechner, der anhand der Nährwertangaben eines Lebensmittels den entsprechenden NutriScore berechnet. Der NutriScore ist ein Lebensmittelkennzeichnungssystem, das in einigen Ländern Europas verwendet wird, um die Nährwertqualität von Lebensmitteln auf der Verpackung darzustellen und Verbrauchern eine einfache Orientierungshilfe für eine gesunde Ernährung zu bieten.

## Funktionsweise

Der NutriScore wird anhand der folgenden Nährwertangaben berechnet:

- Brennwert/Energie in kcal
- Fett
- Gesättigte Fettsäuren
- Zucker
- Salz
- Ballaststoffe
- Proteine
- Obst, Gemüse, Hülsenfrüchte, Nüsse, Ölsaaten (nur für bestimmte Produktgruppen relevant)

Das Projekt ist in der Lage, den NutriScore für verschiedene Produktgruppen zu berechnen, darunter "Allgemein", "Wasser", "Getränke", "Käse" und "Fette, Öle & Sahne". Die Berücksichtigung der Produktgruppe ermöglicht eine präzisere Berechnung des NutriScores, da bestimmte Kategorien spezifische Kriterien haben können.

## Verwendung

Um den NutriScore für ein Lebensmittel zu berechnen, rufe die Funktion `calculateNutriScore` auf und übergebe die entsprechenden Nährwertangaben als Parameter. Das Ergebnis ist der berechnete NutriScore, der als Buchstabe (A bis E) ausgegeben wird.

Beispiel:

```javascript
const energy_kcal = 92;
const saturatedFat = 1.4;
const sugar = 3.4;
const salt = 0.79;
const fiber = 0;
const proteins = 11;
const fruitsVegetablesNuts = 0;
const productGroup = "'general'";

const nutriScore = calculateNutriScore(energy_kcal, saturatedFat, sugar, salt, fiber, proteins, fruitsVegetablesNuts, productGroup);
console.log("Der Nutri-Score beträgt: " + nutriScore);
```

Bitte stelle sicher, dass die angegebenen Nährwertangaben in den entsprechenden Einheiten vorliegen (z. B. kJ für Energie und Gramm für Fett, Zucker, etc.).

## Produktgruppen
Für die Berechnung des NutriScores ist es wichtig, die richtige Produktgruppe anzugeben. Hier sind die verfügbaren Produktgruppen und ihre Verwendung:

- "Allgemein (general)": Für allgemeine Lebensmittel ohne spezifische Kategorie.
- "Wasser (water)": Für Wasser ohne zusätzliche Nährstoffe oder Zusatzstoffe.
- "Getränke (beverage)": Für Getränke, die nicht unter "Wasser" fallen.
- "Käse (cheese)": Für Käseprodukte.
- "Fette, Öle & Sahne (fats)": Für Lebensmittel, die hauptsächlich aus Fett und/oder Sahne bestehen.

Stelle sicher, dass du die richtige Produktgruppe entsprechend dem Lebensmittel auswählst.

## Mitwirken

Wir freuen uns über jede Mitwirkung und jeden Beitrag zu diesem Projekt. Falls du einen Fehler gefunden hast, eine Verbesserung vorschlagen möchtest oder eine neue Funktion hinzufügen möchtest, öffne bitte ein Issue oder einen Pull Request auf GitHub.

## Hinweis zur Genauigkeit

Bitte beachte, dass der berechnete NutriScore eine vereinfachte Version ist und nicht alle Feinheiten des offiziellen Nutri-Score-Systems berücksichtigt. Die Genauigkeit der Berechnung hängt auch von der Verfügbarkeit und Richtigkeit der Nährwertdaten ab. Wir übernehmen keine Gewähr für die Richtigkeit der berechneten NutriScores und empfehlen, die Ergebnisse bei Bedarf zu überprüfen.

## Rechtlicher Hinweis

Die Verwendung dieses NutriScore-Rechners erfolgt auf eigene Verantwortung. Wir übernehmen keine Haftung für die Verwendung der berechneten NutriScores oder daraus resultierende Handlungen.

## Kontakt

Bei Fragen oder Anregungen kannst du uns gerne kontaktieren:

- E-Mail: [suvorov.andreas@gmail.com](mailto:suvorov.andreas@gmail.com)
- GitHub: [https://github.com/AndreasSuvorov](https://github.com/AndreasSuvorov)

Wir freuen uns über dein Interesse an diesem Projekt und hoffen, dass es dir bei deinen Ernährungsentscheidungen behilflich ist. Viel Spaß beim Verwenden!
