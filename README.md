# 🎓 SlideToLaTeX Transcriber

Questo script Python automatizza la conversione di slide universitarie in documenti LaTeX. Supporta sia file **PowerPoint (.pptx)** che **PDF**, estraendo il testo e posizionando le immagini nel punto corretto del documento finale.

## 🌟 Caratteristiche
- **Dual Engine**: Riconoscimento automatico e gestione di file `.pdf` e `.pptx`.
- **Image Extraction**: Estrae le immagini dalle slide e le salva in una cartella locale.
- **Auto-Formatting**: Genera un preambolo LaTeX completo con i pacchetti necessari (`graphicx`, `hyperref`, etc.).
- **Interfaccia Interattiva**: Scegli quale file convertire e come chiamare l'output direttamente dal terminale.

---

## 🛠️ Installazione Rapida (Linux/WSL)

Apri il terminale nella cartella del progetto (`transcriver-notes`) ed esegui questi comandi in ordine:

### 1. Crea e attiva l'ambiente virtuale
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 2. Installa le dipendenze
```bash
pip install python-pptx pymupdf
```
### 3. Come si usa?
1. Inserisci le slide: Trascina i tuoi file .pdf o .pptx nella cartella transcriver-notes.

2. Esegui lo script: (dal terminale con ambiente attivo)

```bash

python slides_to_latex.py
```
### Segui le istruzioni:

1. Seleziona il numero corrispondente al file che vuoi convertire.

2. Digita il nome che vuoi dare al file finale (es. Lezione_01).

### 📄 Risultato e Compilazione
Verrà creata una cartella images/ con tutte le figure estratte.
Verrà generato il tuo file .tex personalizzato.

### Puoi compilare il documento caricando l'intero contenuto della cartella su Overleaf o usando un compilatore locale come TeX Live.

📂 Struttura del Progetto
```Plaintext
transcriver-notes/
├── .venv/               # Ambiente virtuale Python
├── images/              # Immagini estratte dalle slide
├── slides_to_latex.py   # Script principale
├── *.tex                # I tuoi file LaTeX generati
└── README.md            # Questa guida
```
Sviluppato per rendere lo studio universitario un po' più smart. 🚀