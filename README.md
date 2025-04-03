# 🐾 Faunalyze

**Faunalyze** is a scientific data pipeline that automates the search and analysis of animal species mentions in peer-reviewed literature.
It leverages trusted APIs like Scopus, Web of Science, and GBIF to create structured datasets for taxonomic and ecological research.

---

## 🚀 Features

- 🔍 Search articles by species name (scientific or common)
- 📄 Extract abstracts, DOIs, authors, and keywords
- 🌿 Enrich results with taxonomic and occurrence data from GBIF
- 📊 Generate structured CSVs for downstream analysis
- 🧪 Built with [Hy](https://hylang.org/) — a LISP dialect embedded in Python

---

## 📦 Project Structure

```
faunalyze/
├── species_search.hy       # Query Scopus for articles mentioning species
├── gbif_lookup.hy          # Lookup taxonomy and distribution via GBIF
├── analysis.hy             # Analysis tools (word clouds, stats, trends)
├── utils.hy                # Helper functions
├── main.hy                 # Entry point to run the pipeline
├── pybliometrics.cfg       # Config file for Scopus access
├── requirements.txt        # Python/Hy dependencies
└── README.md               # You're here :)
```

---

## 📥 Installation

```bash
# clone the repository
$ git clone https://github.com/your-username/faunalyze.git
$ cd faunalyze

# create virtual environment
$ python -m venv .venv
$ source .venv/bin/activate  # Windows: .venv\Scripts\activate

# install dependencies
$ pip install -r requirements.txt
```

---

## 🧪 Usage Example

```bash
# Run the pipeline for a given species
$ hy main.hy
```

Inside `main.hy`, you can change the species to query (e.g. "Panthera leo").

---

## 📄 Requirements

- Python 3.9+ (use `pyenv` or `venv` to manage versions)
- Hy 0.26+
- Access to Scopus API (via [pybliometrics](https://pybliometrics.readthedocs.io/en/stable/))
- Optionally: GBIF public API (no key needed)

---

## 📚 License

MIT License. See [LICENSE](LICENSE) file for details.

---

## 🌱 Future Plans

- [ ] Add async support for faster data collection
- [ ] Integrate PubMed as an alternative source
- [ ] Visualization module (matplotlib/seaborn)
- [ ] Dockerized version for reproducible runs

---

**Made with 🧠 and 🐍 in Hy by GDX and Anna Farias**
