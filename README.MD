# StrokeSegLab Documentation Guide

This document explains how to generate and publish the **HTML API documentation** for the StrokeSegLab project using [pdoc](https://pdoc.dev).

---

## 📦 Requirements

Make sure you have Python ≥ 3.8 and `pdoc` installed:

```bash
pip install pdoc
```
# 🏗️ Generating the Documentation

From the parent directory of the project (the one that contains the StrokeSegLab/ folder):

```bash
PYTHONPATH=StrokeSegLab pdoc -o docs StrokeSegLab
```

This command

   - Tells pdoc to document the StrokeSegLab package.

   - Sets the Python path so internal imports work correctly.

   - Outputs all generated HTML files into the docs/ folder.

After running, your structure will look like this:
```
StrokeSegLab/
├── StrokeSegLab/
│   ├── inference/
│   ├── managers/
│   ├── utils/
│   └── ...
├── docs/
│   ├── index.html
│   ├── inference/
│   ├── managers/
│   ├── preprocessing/
│   └── utils/
└── README.md
```