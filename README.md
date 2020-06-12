# Citing software.

This repository contains a guide on how to cite standard software used by the Glotzer lab at the University of Michigan.
The repository contains a Bibtex bib file suitable for direct copying into the bibliography for any paper.
It includes standard tools in the SciPy stack as well as more specific tools for used by the Glotzer group at the University of Michigan.
A minimal LaTeX file is included to simplify the generation of a PDF (included in the repo as ``citations.pdf``) with formatted citations in case a fully formatted citation is needed for copying into a document editor like Microsoft Word.

Some general guidelines:

* Almost all papers in our group should include citations of NumPy and HOOMD-blue.
* Most papers should also cite signac.
* Most group members use Matplotlib for plot generation and should cite it.
* Users of freud and HOOMD-blue should check the lists below to make sure that you are also citing the papers corresponding to specific features. Common examples include HPMC, PMFTs, and environment matching.
* Pandas, SciPy, and Scikit-learn are commonly used for specific applications, so if you use them in your research please copy those citations from below.
* Anyone directly performing quaternion operations in their scripts should cite rowan.

# Recommended in-text citations

The following are sentences that can be reasonably copy-pasted into either the introduction, conclusion, or acknowledgments section of a LaTeX manuscript (assuming ``citations.bib`` is copied into the paper's bibliography file).

* This work makes use of NumPy \cite{Oliphant2006, vanderWalt2011} and simulations were conducted using the HOOMD-blue simulation toolkit \cite{Anderson2008, Anderson2020, Glaser2015a}.
* All figures in this paper were generated with Matplotlib \cite{Hunter2007} unless otherwise noted.
* Data and workflows were managed using the signac framework \cite{Adorf2018a,Ramasubramani2018b}

# Specific software citations

The following lists provide the LaTeX citation keys that should be used for each document.

## SciPy Stack

* **NumPy**: Oliphant2006, vanderWalt2011
* **Matplotlib**: Hunter2007
* **SciPy**: Virtanen2020
* **Pandas**: McKinney2010
* **Scikit-learn**: Pedregosa2011
* **Cython**: Behnel2011
* **Mayavi**: Ramachandran2011 
* **TensorFlow**: tensorflow2015-whitepaper

## HOOMD-blue

The generic HOOMD-blue citations (the first line below) should be used in any paper that uses HOOMD-blue.
The following citations are feature-specific and should be included based on what features of HOOMD-blue are used in a given manuscript.

* **HOOMD-blue**: Anderson2008, Anderson2020, Glaser2015a
* **HPMC**: Anderson2016
* **Depletion**: Glaser2015b
* **DEM**: Spellings2017
* **Rigid bodies**: Nguyen2011, Glaser2020
* **PPPM**: Lebard2012
* **DPD**: Phillips2011

## signac

* Adorf2018a, Ramasubramani2018b

## freud

The generic freud citation should be used in any paper that uses freud.
The following citations are feature-specific and should be included based on what features of freud are used in a given manuscript.

* **freud**: Ramasubramani2020
* **ML/visualization**: Dice2019
* **Steinhardt OPs**: Steinhardt1983
* **Neighbor-averaged Steinhardt OPs**: Lechner2008
* **PMFTs**: VanAnders2014c, vanAnders2014d
* **Environment Matching**: Teich2019
* **MSDs**: Calandrini2011
* **Voronoi**: Rycroft2009
* **Cubatic OP**: Haji-Akbari2015
* **Rotational autocorrelation**: Karas2019

## rowan

* Ramasubramani2018


# Contributing

To add new citations, update the ``citations.bib`` file.
The citation key should be in AuthorYear format (with additional letters as needed, e.g. "Anderson2018a").
If the citation is related to an existing software package such as a new feature for HOOMD-blue, it should be placed in the appropriate section of the bib file.
Then, update the [Specific Software Citations](#specific-software-citations) section of this document.
As a convenience, rerun LaTeX on the provided tex file to regenerate the PDF containing formatted citations.

# License

Written in 2020 by Vyas Ramasubramani (<vramasub@umich.edu>).
To the extent possible under law, the author(s) have dedicated all copyright and related and neighboring rights to the public domain worldwide.
This content is distributed without any warranty.
You should have received a copy of the CC0 Public Domain Dedication along with this repository.
If not, see <http://creativecommons.org/publicdomain/zero/1.0/>.
