# DocFGP Latin

[![PyPI version](https://img.shields.io/pypi/v/docfgp-latin)](https://pypi.org/project/docfgp-latin/)
[![PyPI downloads](https://img.shields.io/pepy/dt/docfgp-latin)](https://pepy.tech/projects/docfgp-latin)
[![CI](https://github.com/docfgp/docfgp-latin/actions/workflows/ci.yml/badge.svg)](https://github.com/docfgp/docfgp-latin/actions/workflows/ci.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/docfgp/docfgp-latin)](LICENSE)

DocFGP Latin provides the [tessdata_fast](https://github.com/tesseract-ocr/tessdata_fast) Tesseract models that let [DocFGP](https://github.com/docfgp/docfgp) OCR the Latin script.

## Requirements

- Python 3.11+

## Installation

```bash
pip install docfgp
```

## Usage

```python
from docfgp import FingerprintConfig, Fingerprinter

fingerprinter = Fingerprinter(FingerprintConfig(ocr_language="eng+deu"))
fingerprint = fingerprinter.fingerprint("scan.pdf")
```

| Model | `ocr_language` values |
| --- | --- |
| `eng` | `eng` |
| `script/Latin` | `afr`, `aze`, `bos`, `bre`, `cat`, `ceb`, `ces`, `cos`, `cym`, `dan`, `deu`, `epo`, `est`, `eus`, `fao`, `fil`, `fin`, `fra`, `fry`, `gla`, `gle`, `glg`, `hat`, `hrv`, `hun`, `ind`, `isl`, `ita`, `jav`, `lat`, `lav`, `lit`, `ltz`, `mlt`, `mri`, `msa`, `nld`, `nor`, `oci`, `pol`, `por`, `que`, `ron`, `slk`, `slv`, `spa`, `sqi`, `srp_latn`, `sun`, `swa`, `swe`, `ton`, `tur`, `uzb`, `yor` |
