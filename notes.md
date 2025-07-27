Dataset:
https://github.com/nelson-liu/evaluating-verifiability-in-generative-search-engines
Paper
- Internal + External interpolation (Bei Komplementären Informationen)
- LLM soll zeigen, dass Knowledge interpoliert wird


RQ 1:
How can we use LLM-based reasoning to decide whether the information from the retrieved documents is relevant, correct , and complete to generate a comprehensive response to a query?

- wissensch. Fragestellung die mehr Wissen brauchen als gegeben z.B. "welches LLM ist gut?" -> schlägt nur aktuelle vor, aber antwort sollte alle aktuelle vorschlagen. Ein llm sagt dann o4, llama etc, aber eig sollte mehr abgewogen werden


1. Schritt
- Dataset (aus paper) anschauen; Hat DS golden Answers?
- Was macht LLM von sich aus, wenn nicht expl. (interpol.)
2. Schritt
- DS aufbereiten
-. z.B. Fakten rausnehmen -> wie interpoliert LLM?
- weiß LLM Fakt, den er interpolieren soll? (Knowledge probing Ansätze)
--> Wen Fakt raus --> kannte llm fakt?


Stichwort „knowledge probing“ für die Überprüfung des Wissens eines LLMs.
Knowledge Probing: Testen, ob das LLM einen Fakt kennt, wenn er im Kontext fehlt.
Besitzt das LLM selbst dieses Wissen in seinen Gewichten, oder hängt es von externen Quellen (RAG) ab
Die Probe ist dabei oft so formuliert, dass keine Suche, kein Kontext verwendet wird sondern nur das Modellwissen zählt.
--> Also source_text entfernen
z.b.
  source_text = "Paris is the capital of France"
  query = "What is the capital of France?"
  statement = "Paris is the capital of France"
  label = "correct"
  prediction = "correct"
  match = True











