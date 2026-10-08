Analizza il file Excel e individua tutte le anomalie presenti.

Restituisci il risultato esclusivamente in forma tabellare con le colonne:

| Foglio | Scheda/Riga | Campo | Valore trovato | Tipo di anomalia | Motivazione |

Tipi di anomalia ammessi:
- Valore fuori scala
- Errore di formato
- Errore di unità di misura
- Dato mancante
- Duplicato incoerente
- Incoerenza logica
- Errore di calcolo
- Errore di data

Regole:
- Non correggere i dati.
- Non inventare informazioni mancanti.
- Evidenzia anche le anomalie potenziali se motivate dal confronto con il resto del dataset.
- Al termine indica il numero totale di anomalie trovate.

Esempio di output:

| Foglio | Scheda | Campo | Valore trovato | Tipo | Motivazione |
|---------|---------|---------|---------|---------|---------|
| Concept | CS-03 Libeccio | Lunghezza | 2400 m | Valore fuori scala | Tutte le altre unità hanno lunghezze comprese tra 16 e 24 m |
| Registro | Riga 12 | Data | 13/13/2026 | Errore di data | Il mese 13 non esiste |
| Pesi_CS01 | Totale | 70000 kg | Errore di calcolo | La somma delle voci produce 73700 kg |
