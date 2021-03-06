# BIOMD0000000402: Ayati2010_BoneRemodelingDynamics_WithTumour

## Installation

Download this repository, and install with distutils

`python setup.py install`

Or, install using pip

`pip install git+https://github.com/biomodels/BIOMD0000000402.git`

To install a specific version (in this example, from the 2014-09-16 BioModels release)

`pip install git+https://github.com/biomodels/BIOMD0000000402.git@20140916`

## Usage

Importing the model package.

`import BIOMD0000000402 as model`

Get the SBML string from the model

`print model.sbmlString`

If [python-libsbml](https://pypi.python.org/pypi/python-libsbml) bindings are
installed, the libsbml.SBMLDocument object is also accessible

`model.sbml`


# Model Notes


This a model from the article:  
** A mathematical model of bone remodeling dynamics for normal bone cell populations and myeloma bone disease **   
Bruce P Ayati, Claire M Edwards, Glenn F Webb and John P Wikswo. _Biology
Direct_2010 Apr 20;5(28).
[20406449](http://www.ncbi.nlm.nih.gov/pubmed/20406449),  
**Abstract:**   
BACKGROUND: Multiple myeloma is a hematologic malignancy associated with the
development of a destructive osteolytic bone disease. RESULTS: Mathematical
models are developed for normal bone remodeling and for the dysregulated bone
remodeling that occurs in myeloma bone disease. The models examine the
critical signaling between osteoclasts (bone resorption) and osteoblasts (bone
formation). The interactions of osteoclasts and osteoblasts are modeled as a
system of differential equations for these cell populations, which exhibit
stable oscillations in the normal case and unstable oscillations in the
myeloma case. In the case of untreated myeloma, osteoclasts increase and
osteoblasts decrease, with net bone loss as the tumor grows. The therapeutic
effects of targeting both myeloma cells and cells of the bone marrow
microenvironment on these dynamics are examined. CONCLUSIONS: The current
model accurately reflects myeloma bone disease and illustrates how treatment
approaches may be investigated using such computational approaches.

**Note:**

The paper describes three models 1) Zero-dimensional Bone Model without
Tumour, 2) Zero-dimensional Bone Model with Tumour and 3) Zero-dimensional
Bone Model with Tumour and Drug Treatment. This model corresponds to the Zero-
dimensional Bone Model with Tumour.

Typos in the publication:

Equation (4): The first term should be (β1/α1)^(g12/Γ) and not (β2/α2)^(g12/Γ)

Equation (14): The first term should be (β1/α1)^(((g12/(1+r12))/Γ) and not
(β2/α2)^(((g12/(1+r12))/Γ)

Equation (13): The first term should be (β1/α1)^((1-g22+r22)/Γ) and not
(β1/α1)^((1-g22-r22)/Γ)

All these corrections has been implemented in the model, with the authors
agreement.

Beyond these, there are several mismatches between the equation numbers that
are mentioned in for each equation and the reference that has been made to
these equations in the figure legend.


