# The Metabolic Disassembler

The Metabolic Disassembler is a Python package to automatically predict a combination of biosynthetic units in a natural product. This software would help to reveal the starting materials of the target natural product.  


## Installation

Install The Metabolic Disassembler with `pip`.  
  
```bash
$ pip install metadisassembler
```

## Requirements

- Python (3.6)
  - [RDKit](https://www.rdkit.org)(version 2018.09.1.0)
  - [NetworkX](https://networkx.github.io/documentation/stable/)(version 2.2)
  - [CairoSVG](https://cairosvg.org)(version 2.2.1)
  - [Pillow (PIL)](https://pillow.readthedocs.io/en/stable/)
  - [Pandas](https://pandas.pydata.org)
  - [Matplotlib](https://matplotlib.org)

## Command Line Usage


```bash
% metadisassembler -h
usage: metadisassembler [-h] [-t TIME] [--hide] [-c] [-p] query

positional arguments:
  query                 MDL_Molfile, SMILES, InChI, KEGG_COMPOUND_ID,
                        KNApSAcK_COMPOUND_ID

optional arguments:
  -h, --help            show this help message and exit
  -t TIME, --time TIME  set a time limit [s] [default: 300]
  --hide                hide stereochemistry [default: False]
  -c, --color           output color allocation information [default: False]
  -p, --pro             you never miss any combination (NOT RECOMMENDED).
                        [default: False]
```

## Basic Usage
An example notebook is available [here](https://github.com/the-metabolic-disassembler/metadisassembler/blob/master/jupyter_usecase/basic_usage.ipynb).   
   
You can try it in Google Colab. [![colab-logo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/the-metabolic-disassembler/metadisassembler/blob/master/jupyter_usecase/basic_usage_in_colab.ipynb)
