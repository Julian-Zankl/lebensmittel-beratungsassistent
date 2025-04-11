# Lebensmittel-Beratungsassistent

## Projektbeschreibung

Der Lebensmittel-Beratungsassistent ist eine KI-gestützte Anwendung, die
Nutzer:innen personalisierte Ernährungsempfehlungen bietet. Basierend auf
individuellen Angaben wie Alter, Geschlecht, Körpergröße, Essgewohnheiten und
Allergien kann das System passende Diätvorschläge und Beispiel-Tagespläne
generieren.

## Zielsetzung

Das Ziel dieses Projekts ist es, eine Conversational AI zu entwickeln, die
Nutzer:innen bei Ernährungsfragen unterstützt. Dabei werden relevante Daten mit
einer RAG (Retrieval-Augmented Generation)-Komponente verarbeitet, um gezielte
Antworten aus einer Wissensbasis zu liefern.

## Funktionen

- **Personalisierte Ernährungsempfehlungen** basierend auf Nutzereingaben
- **Berechnung des BMI und Kalorienbedarfs**
- **Beratung zu geeigneten Diäten** (z. B. Low Carb, Vegan, Paleo)
- **Allergie-Check und Kontraindikationen**
- **Abruf von Beispiel-Tagesplänen für verschiedene Ernährungstypen**

## Technische Umsetzung

### Genutzte Technologien

- **Python** für die Implementierung
- **Jupyter Notebook** für die Entwicklungsumgebung
- **RAG-Komponente** zur Wissensabrufung
- **OpenFoodFacts API** zur Abfrage von Lebensmittelinformationen
- **Vektor-Datenbank (Milvus Lite)** für Embedding-gestützte Suchanfragen

### Architektur

1. **Datensammlung:** Ernährungsempfehlungen, Diätpläne und wissenschaftliche
   Quellen werden in ein PDF-Dokument zusammengeführt.
2. **Datenverarbeitung:** Parsing und Chunking der Dokumente für die
   RAG-Komponente.
3. **Einbettung in eine Vektor-Datenbank:** Um relevante Informationen abrufen
   zu können.
4. **Agentensteuerung:** Ein KI-Agent analysiert Nutzeranfragen und nutzt die
   RAG-Komponente zur Generierung der besten Antwort.

## Installation & Setup

### Voraussetzungen

- Python 3.11+

## Nutzung

1. Notebook öffnen und die ersten Zellen ausführen, um das Modell und die Daten
   zu laden.
2. In der interaktiven Chat-Umgebung Eingaben machen (z. B. "Welche Diät passt
   zu einem aktiven Lebensstil?").
3. Ergebnisse werden basierend auf den vektorisierten Informationen aus der
   RAG-Komponente generiert.
