# atlantic-causal-2017
Entry for the Atlantic Causal Inference Conference's 2017 competition

## Requirements

* R 3.2 or later.
* java

## How to run

* Unzip [2016 data](https://drive.google.com/file/d/0B8TUkApaUlsGekFSblJWa25NM1E/edit) into inbound/data-2016/
* To run analyses without using SLURM job submission, set an environmental variable in BASH (or add to ~/.bashrc):

```bash
export USE_JOBS=shell
```
* Run setup.R to install the necessary packages: `make setup`
* Run import-2016.R to import the 2016 data: `make import-2016`
* Run test-2016.R to conduct a single test analysis of 2016: `make test-2016`
* Run analyze-2016.R to analyze all 2016 files using targeted_learning.R: `make analyze-2016`

## Subdirectory layout

(This can evolve as we go.)

* Archive - old source code that is saved for reference.
* Data - working RData files generated during analysis, not tracked via git.
* Exports - exported files (cvs, tsvs, etc.) that are not tracked via git.
* Inbound - input datasets that are not tracked via git.
* Lib - R source code that defines functions; all .R files are loaded.
* Output - log output files from Savio jobs  etc.
* Scripts - shell (BASH) scripts.
* Tex - tex output
* Writeup - analysis reports and memos
