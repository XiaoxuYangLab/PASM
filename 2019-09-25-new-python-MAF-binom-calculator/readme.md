# Python version of PASM

Implemented by Xin Xu with input from Xiaoxu Yang and all the previous versions of scripts, maintained by Xin Xu and Xiaoxu Yang.

## Before starting:
[NumPy](https://numpy.org/), [pandas](https://pandas.pydata.org/), and [scipy](https://www.scipy.org/) packages should be available for your Python.

## Usage of the tool:
`python new_compute_binom.py <CHR> <POS> <REF> <ALT> <BAM_PATH>`

## Output format:
`python new_compute_binom.py <Depth> <Ref+Alt> <Aa_count> <Aa_count> <Cc_count> <Gg_count> <Tt_count> <insertion_count> <deletion_count> <insertion_alt_count> <deletion_alt_count> <num_alt/(num_ref+num_alt)> <95%binomial_CI_lower> <95binomial_CI_higher> <p-value of Fisher strand bias>

## Notes: 
You can edit the script in order to switch the methods to calculate confidence intervals ([PASM CI](https://doi.org/10.1002/humu.22819), [Clopper-Pearson exact binomial CI, and Wilson score CI](https://en.wikipedia.org/wiki/Binomial_distribution#Confidence_intervals)).
