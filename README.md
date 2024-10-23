# NLP-SentimentAnalysis

In diesem Projekt soll analysiert werden, wie die politische Berichterstattung im Standard mit NLP-Methoden analysiert werden können. Zunächst wird eine Datenbank modelliert. Anschließend wird diese SQLite Datenbank mithilfe der mit Webscraping gesammelten Artikel vom Standard befüllt. Danach folgt ein Feature Engineering Teil, wo wir die Sentiments, keywords, etc. ermitteln, um sie im Analyseteil zum Aggregieren zu verwenden.

Es werden auch einige Kommentare gescraped und mittels eines Emotion-Klassifikationsmodells untersucht.

Die Jupyter-Notebooks sind in der folgenden Reihenfolge zu berücksichtigen:
1) **derstandard_tracker.txt** – Dient dazu, die bereits gescrapten Artikel tageweise zu verfolgen
2) **scraper.ipynb** – Scraper um die Artikel zu erhalten
3) **scrape_comments_19102024.ipynb** – Scraper um die Kommentare der Artikel zu erhalten
4) **migration zu neuen DB struktur.ipynb** – Gescrapte Daten werden in einem neuen Datenbankstruktur übertragen
5) **auswertung.ipynb** – Anlegen der gesuchten Keywords (Parteien), vorläufige Abfragen
6) **FeatureEngineering_Final_13102024.ipynb** – Erstellung der Feature-Tabelle in der Datenbank mit Features wie Satzanzahl, Wortanzahl, durchschnittliche Wortlänge, Anzahl der Token
7) **Sentiment_Voranalyse_10102024.ipynb** – Vorläufige Chunk-Einführung und Sentimentanalyse
8) **Sentiment_Final_13102024.ipynb** – Finale Sentimentanalyse der Artikel
9) **Emotion_Final_19102024.ipynb** – Emotionsanalyse der Kommentare der Artikel
10) **Dataviz_Final_19102024.ipynb** – Visualisierung der Ergebnisse der Sentiment- und Emotionsanalysen

Weitere Dateien:
- **ERM Ordner** – Abbildung des Entity Relationship Model
- **Requirements.txt** – Liste der notwendigen Libraries/Packages
