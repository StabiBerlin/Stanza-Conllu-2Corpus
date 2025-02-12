# Stanza-Conllu-2Corpus
 Convert text files with Stanza (NLP) to AntConc-Format for different languages

# Stanza-based Processing of Church Slavonic and Classical Texts

This repository contains a collection of scripts for the automatic processing and annotation of Church Slavonic, Latin, and Ancient Greek corpus materials using **Stanza**. These scripts were developed as part of the training on **Corpus Linguistics in Slavic Studies** (Online-Workshop [1](https://blog.sbb.berlin/termin/slawische-historische-texte-23-1-25/), [2](https://blog.sbb.berlin/termin/kirchenslavica-10-2-25/))and enable the automatic analysis of texts with modern NLP methods.

## Overview
The scripts cover the entire text processing pipeline:

1. **TXT → CoNLL-U**: Conversion of plain text files into CoNLL-U format with lemmatization, POS tagging, and dependency parsing.
2. **CoNLL-U → POS**: Extraction of POS-tagged text from CoNLL-U files for a simplified view.
3. **CoNLL-U → SQLite**: Storage of CoNLL-U data in an SQLite database for structured analysis.

## Included Scripts

| File | Description |
|--------|-------------|
| `stanza-txt-2-conllu-grc.ipynb` | Converts Ancient Greek texts into CoNLL-U format |
| `stanza-txt-2-conllu-lat.ipynb` | Converts Latin texts into CoNLL-U format |
| `stanza-txt-2-conllu-chu.ipynb` | Converts Church Slavonic texts into CoNLL-U format |
| `stanza-conllu-2-pos-grc.ipynb` | Extracts POS annotations from Ancient Greek CoNLL-U |
| `stanza-conllu-2-pos-lat.ipynb` | Extracts POS annotations from Latin CoNLL-U |
| `stanza-conllu-2-pos-chu.ipynb` | Extracts POS annotations from Church Slavonic CoNLL-U |
| `stanza-conllu-2-sqlite-grc.ipynb` | Stores Ancient Greek CoNLL-U data in SQLite |

## Requirements
- **Python 3.x**
- **Stanza** (`pip install stanza`)
- **SQLite3** for database handling

## Usage
### 1. Install dependencies
```bash
pip install stanza
```
### 2. Download Stanza models
The required language models can be downloaded using Stanza:
```python
import stanza
stanza.download('grc')  # Ancient Greek
stanza.download('la')   # Latin
stanza.download('cu')   # Church Slavonic
```

### 3. Run the scripts
The Jupyter notebooks can be opened and executed using **Jupyter Notebook** or **Jupyter Lab**:
```bash
jupyter notebook
```

## Contact
This project was created as part of a training session on **Corpus Linguistics in Slavic Studies**. If you have any questions or suggestions, feel free to open an issue or get in touch.

