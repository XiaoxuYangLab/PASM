# RNA version of PASM

Modified from the DNA version, maintained by Xiaoxu Yang and Xincen Xi.

## Before starting:
[scipy](https://www.scipy.org/), [pandas](https://pandas.pydata.org/), and [NumPy](https://numpy.org/) packages should be available for your Python.

## Usage of the tool:
`python new_compute_binom.py <CHR> <POS> <REF> <ALT> <BAM_PATH>`

## Output format:
`python new_compute_binom_RNA.py <Depth> <Ref+Alt> <Aa_count> <Aa_count> <Cc_count> <Gg_count> <Tt_count> <insertion_count> <deletion_count> <insertion_alt_count> <deletion_alt_count> <num_alt/(num_ref+num_alt)> <95%binomial_CI_lower> <95binomial_CI_higher> <p-value of Fisher strand bias>`

## Notes: 
For skipped transcripts, depth will be the same as mpileup but Ref+Alt count will be smaller depending on how many reads skipps the position

You can edit the script in order to switch the methods to calculate confidence intervals ([PASM CI](https://doi.org/10.1002/humu.22819), [Clopper-Pearson exact binomial CI, and Wilson score CI](https://en.wikipedia.org/wiki/Binomial_distribution#Confidence_intervals)).
