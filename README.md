# juicer-rackham
Scripts from Juicer pipeline for analysis of Hi-C data (https://github.com/aidenlab/juicer) modified for use on Rackham / Uppmax.

## Changes

The following changes to the original code were made.

`juicer_rackham.sh`

1. load modules for `bwa` and related available on Rackham;

2. remove some of the Aiden lab specific code;

3. add the currect script name `split_rmdups_rackham.awk ` in the DEDUP step; modify the call to this script to include CPU allocation;

4. correct cmd for DUPCHECK step to include CPU allocation;


`split_rmdups_rackham.awk`

1. correct `sbatch` calls to include CPU allocation;


## Usage

Clone the repository, copy the scripts to `juicer/scripts` and that's it.
