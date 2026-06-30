# 🌍 Rocky Worlds Data Challenge — Exoplanets 6 Hands-on Special Session 
Welcome! In this activity you'll fit JWST secondary eclipses and prepare a submission for the Rocky Worlds Data Challenge.

## 🛠️ 1. Create the environment

First, be sure to clone this repository in your local computer. You can either download the code directly, or you can do, in a terminal, if you have `git`:

```bash
git clone https://github.com/nespinoza/rocky-worlds-data-challenge.git
cd rocky-worlds-data-challenge/tutorials/exoplanets6
```

Alternatively, you can also use `curl`:
```bash
curl -L https://github.com/nespinoza/rocky-worlds-data-challenge/archive/refs/heads/main.zip -o rocky-worlds.zip
unzip rocky-worlds.zip
```

Then, from a terminal, run:

```bash
conda env create -f environment.yml
conda activate rw-exo6
```

This may take a few minutes the first time.

## 📥 2. Download the data

Open and run:

```
1-download-some-data.ipynb
```
i.e., by doing

```
jupyter notebook 1-download-some-data.ipynb
```
in a terminal. Note to run this, you will need to create [a Kaggle account](https://www.kaggle.com/). This downloads the JWST datasets (~40 GB).

## 💻 Short on storage or bandwidth?

No problem! You can complete almost the entire activity without downloading the full datasets.

Skip Notebook 1 and go directly to:

```
2-analyze-some-data.ipynb
```

Near the top of the notebook, change

```python
have_uncal_data = True
```

to

```python
have_uncal_data = False
```

The notebook will then use the included time-series files:

- `ts_gj.txt`
- `ts_lhs.txt`

instead of the raw JWST `*.uncal` observations (for GJ 3929 b) and simulations (for LHS 1140 b).

## 🚀 You're ready!

Open `2-analyze-some-data.ipynb` and enjoy the workshop! To submit your `.zip` output, go to the [Kaggle Rocky Worlds DDT Data Challenge webpage](https://www.kaggle.com/competitions/rocky-worlds-data-challenge/data).
