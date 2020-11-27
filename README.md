# Sample and Data Relationship Format for Proteomics (SDRF-Proteomics)

[![License](https://flat.badgen.net/github/license/bigbio/proteomics-metadata-standard)](https://github.com/bigbio/proteomics-metadata-standard/blob/master/LICENSE)
[![Open Issues](https://flat.badgen.net/github/open-issues/HUPO-PSI/mzSpecLib)](https://github.com/bigbio/proteomics-metadata-standard/issues)
[![Open PRs](https://flat.badgen.net/github/open-prs/bigbio/proteomics-metadata-standard)](https://github.com/bigbio/proteomics-metadata-standard/pulls)
![Contributors](https://flat.badgen.net/github/contributors/bigbio/proteomics-metadata-standard)
![Watchers](https://flat.badgen.net/github/watchers/bigbio/proteomics-metadata-standard)
![Stars](https://flat.badgen.net/github/stars/bigbio/proteomics-metadata-standard)

## Improving metadata annotation of Proteomics datasets

The *Sample and Data Relationship Format for Proteomics (SDRF-Proteomics)* project aims to define a set of guidelines to support the annotation of the sample metadata in in public proteomics experiments. Our goal is to ensure maximum reusability of the deposited data. Our work aims to define the minimum information required to report the experimental design of proteomics experiments, enabling the use and reuse of the deposited data by the proteomics community.

The following _Use Cases_ should be considered to design the Proteomics Experimental design data format:

- The "Sample and Data Relationship Format for Proteomics (SDRF-Proteomics)" complement the [proteomeXchange.xml](http://ftp.pride.ebi.ac.uk/pride/resources/schema/proteomexchange/proteomeXchange-1.4.0.xsd) file format implemented by [ProteomeXchange](http://www.proteomexchange.org/) to capture the minimum metadata about a proteomics dataset. The ProteomeXchange submission XML file format is detailed [here](http://www.proteomexchange.org/docs/guidelines_px.pdf).

- It SHOULD enable data submitters and curators to annotate a proteomics dataset at different levels, including the sample metadata (e.g. organism and tissues), technical metadata (e.g. instrument model) and the experimental design.

- It SHOULD facilitate the automatic reanalysis of public proteomics datasets, by providing a better representation of quantitative data in public repositories.

## SDRF-Proteomics

 - [SDRF-Proteomics](https://github.com/bigbio/proteomics-metadata-standard/tree/master/sdrf-proteomics)

## How to contribute

External contributors, researchers and the proteomics community are more than welcome to contribute to this project.

Contribute with the specification: you can contribute to the specification with ideas or refinements by adding an issue into the [issue tracker](https://github.com/bigbio/proteomics-metadata-standard/issues) or performing a PR.

In the [annotated projects](https://github.com/bigbio/proteomics-metadata-standard/tree/master/annotated-projects) folder the user can see different public datasets that have been annotated so far by the contributors. If you would like to join these efforts, make a Fork of this repo and perform a pull request (PR) with your annotated project. If you don't have a project in mind, you can take one project from the [issues](https://github.com/bigbio/proteomics-metadata-standard/issues) and perform the annotation.

Annotate a dataset in 5 steps:

- Read the [SDRF-Proteomics specification](https://github.com/bigbio/proteomics-metadata-standard/tree/master/sdrf-proteomics)

- Depending on the type of dataset, choose the appropriate [sample template](https://github.com/bigbio/proteomics-metadata-standard/tree/master/sdrf-proteomics#sdrf-templates)

- Annotate the the corresponding ProteomeXchange PXD dataset following the guidelines

- Validate your SDRF:

In order to validate your SDRF, you can install the sdrf-pipelines tool in Python


```bash
pip install sdrf-pipelines
```

validate the SDRF

```bash
parse_sdrf validate-sdrf --sdrf_file sdrf.tsv
```

You can read more about the validator [here](https://github.com/bigbio/sdrf-pipelines).

. Fork the current repository, add a folder with the ProteomeXchange accession and the annotated sdrf.tsv

## Core contributors and collaborators

The project is run by different groups:

- Yasset Perez-Riverol (PRIDE Team, European Bioinformatics Institute - EMBL-EBI, U.K.)
- Timo Sachsenberg (OpenMS Team, Tübingen University, Germany)
- Anja Fullgrabe (Expression Atlas Team, European Bioinformatics Institute - EMBL-EBI, U.K.)
- Nancy George (Expression Atlas Team, European Bioinformatics Institute - EMBL-EBI, U.K.)
- Mathias Walzer (PRIDE Team, European Bioinformatics Institute - EMBL-EBI, U.K.)
- Pablo Moreno (Expression Atlas Team, European Bioinformatics Institute - EMBL-EBI, U.K.)
- Juan Antonio Vizcaíno (PRIDE Team, European Bioinformatics Institute - EMBL-EBI, U.K.)
- Oliver Alka (OpenMS Team, Tübingen University, Germany)
- Julianus Pfeuffer (OpenMS Team, Tübingen University, Germany)
- Marc Vaudel (University of Bergen, Norway)
- Harald Barsnes (University of Bergen, Norway)
- Niels Hulstaert (Compomics, University of Gent, Belgium)
- Lennart Martens (Compomics, University of Gent, Belgium)
- Expression Atlas Team (European Bioinformatics Institute - EMBL-EBI, U.K.)
- Lev Levitsky (INEP team, INEPCP RAS, Moscow, Russia)
- Elizaveta Solovyeva (INEP team, INEPCP RAS, Moscow, Russia)
- Stefan Schulze (University of Pennsylvania, USA)
- Veit Schwämmle (Protein Research Group, University of Southern Denmark, Denmark)
- ProteomicsDB Team (Technical University of Munich, Germany)
- David Bouyssié (ProFI/IPBS, University of Toulouse, CNRS, Toulouse, France)
- Nicholas Carruthers (Wayne State University, USA)
- Paul Rudnick (NCI, Proteomic Data Commons, USA)
- Enrique Audain (University Medical Center Schleswig-Holstein, Germany)
- Marie Locard-Paulet (Novo Nordisk Foundation Center for Protein Research, University of Copenhagen, Denmark)
- Johannes Griss (Department of Dermatology, Medical University of Vienna, Austria)
- Chengxin Dai (Chongqing Key Laboratory on Big Data for Bio Intelligence, Chongqing University of Posts and telecommunications, Chongqing, China)
- Julian Uszkoreit ( Medical Faculty, Medizinisches Proteom-Center and Center for Protein Diagnostics (PRODI), Medical Proteome Analysis, Ruhr-University Bochum, Germany)
- Dirk Winkelhardt ( Medical Faculty, Medizinisches Proteom-Center and Center for Protein Diagnostics (PRODI), Medical Proteome Analysis, Ruhr-University Bochum, Germany)
- Kanami Arima (Toyama University of International Studies, Toyama, Japan)
- Shin Kawano (Toyama University of International Studies, Toyama, Japan)

IMPORTANT: If you contribute with the following specification, please make sure to add your name to the list of contributors.

## Code of Conduct

As part of our efforts toward delivering open and inclusive science, we follow the [Contributor Covenant Code of Conduct for Open Source Projects](https://www.contributor-covenant.org/version/2/0/code_of_conduct/).

## How to cite

Perez-Riverol, Yasset, European Bioinformatics Community for Mass Spectrometry. "Towards a sample metadata standard in public proteomics repositories." Journal of Proteome Research (2020) [Manuscript](https://pubs.acs.org/doi/abs/10.1021/acs.jproteome.0c00376).

## Copyright notice


    This information is free; you can redistribute it and/or modify it
    under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.

    This information is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this work; if not, write to the Free Software
    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.
