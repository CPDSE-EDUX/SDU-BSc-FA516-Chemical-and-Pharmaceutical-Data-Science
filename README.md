# FA516: Chemical and Pharmaceutical Data Science

**Part of [CPDSE](https://cpdse.dk): Center for Pharmaceutical Data Science Education.**
Bachelor course in chemistry and pharmacy, University of Southern Denmark.

## About This Repository

This repository holds the **exercises** for FA516: the notebooks you
open, run and fill in. The complete course material (videos, quizzes, slides, deadlines,
and the project description) lives in itslearning.

Solutions are not published here. They are worked through in class and handed out
afterwards.

## How the Course Works

The course is *not* a sequence of lectures. It is **eight tracks**, and every track works
the same way.

Tracks 1-6 are mandatory and build on each other: Python fundamentals, data science
foundations, cheminformatics, statistical learning, classification, and machine learning
workflows. Tracks 7 and 8, deep learning and generative modelling, are **voluntary**.
Nobody is examined in them.

Each mandatory track has the same rhythm:

| | |
|---|---|
| **Prepare** | Before each class: watch the short videos, work the small self-study exercise from `prepare/`, take the topic quiz in itslearning. Plan 60-90 minutes, roughly half an hour each. |
| **Class** | Two hours, twice per track, twelve classes in all. One large worksheet from `class/`, worked at your own machine with the teacher in the room. |
| **Self-study** | Everything after: deeper reading, larger exercises, and the work that feeds into the group project. |

**The scaffolding falls away**: in track 1 most of the code is already written and you
complete expressions; by tracks 5 and 6 only the opening is given and the rest is yours.
The same happens inside each worksheet, from filling in a value in part 1 to writing a
function from scratch in the last.

The exam is a group project (3-4 students): a single [Jupyter](https://jupyter.org/)
notebook covering dataset curation, exploratory analysis, molecular features, at least one
machine learning model, evaluation and scientific discussion. It must run without
modification.

## Structure

```
├── README.md
├── environment.yml                # the Python environment for the whole course
├── data/                          # datasets an exercise reads but does not create (added when needed)
└── track-N-name/
    ├── README.md                  # what the track covers and what its classes do
    ├── prepare/                   # short self-study exercises, one per video
    └── class/                     # the 2 h in-class worksheets, one per class
```

Tracks appear here as their exercises are finished, so this list grows during the
semester.

| Track | Topics | Classes | Status |
|---|---|---|---|
| [Track 1: Python Fundamentals](track-1-python/) | Python basics, lists & data structures, cheminformatics with Python, NumPy, SciPy and pandas | 2 | mandatory |
| [Track 2: Data Science Foundations](track-2-data-science/) | Chemical data types & formats, preprocessing & cleaning, EDA & visualization | 2 | mandatory |
| [Track 3: Cheminformatics](track-3-cheminformatics/) | SMILES & stereochemistry, molecular descriptors, fingerprints | 2 | mandatory |

Videos are on YouTube, one playlist per track, linked from each track's README and from
itslearning.

## Working the Exercises

The notebooks are **blanked, not empty**. Imports, given data and helper functions are
handed to you complete, so your time goes on learning rather than on retyping
machinery. The lines you write are marked:

```python
mw = _          # the molecular weight of the molecule
# label the x axis
```

Each task is a numbered question directly above the cell it applies to. A question that
says *explain*, *predict* or *what does this print* is answered in words: there is
nothing to fill in. Some cells are meant to fail: read the traceback and repair it.

Every notebook runs top to bottom on its own and needs no file that is not either in
`data/` or created by the notebook itself.

## Setup

You need [Python](https://www.python.org/) with [RDKit](https://www.rdkit.org/),
[pandas](https://pandas.pydata.org/), [NumPy](https://numpy.org/),
[SciPy](https://scipy.org/), [Matplotlib](https://matplotlib.org/),
[scikit-learn](https://scikit-learn.org/) and Jupyter.

```bash
conda env create -f environment.yml
conda activate fa516
jupyter notebook
```

Matplotlib is the only plotting library used in the course.

## License

Written material is licensed [CC BY 4.0](LICENSE); the code in the notebooks is
[MIT](LICENSE-code). See [CITATION.cff](CITATION.cff) for how to cite the course.

Following the CPDSE convention, `main` carries the current edition of the course; each
finished edition is snapshotted to a year branch (`2026`, `2027`, `...`).
