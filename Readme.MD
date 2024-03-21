```
# README: htgts.sh

## Description
The `htgts.sh` script is designed to perform analysis on data obtained from HTGTS (High-Throughput Genome-Wide Translocation Sequencing) experiments. This is a technique used to map genomic translocations on a large scale.

## Usage
```
./htgts.sh <Data_folder> <fastq1> <fastq2> <expInfo> <expInfo2> <outDir>
```

### Arguments
- `<Data_folder>`: The directory containing the required input files for analysis. It's recommended to use the absolute path.
- `<fastq1>`: The FASTQ file containing reads from the first sample.
- `<fastq2>`: The FASTQ file containing reads from the second sample, if available. If not present, leave it empty.
- `<expInfo>`: The experimental information file related to the first sample.
- `<expInfo2>`: The experimental information file related to the second sample, if available. If not present, leave it empty.
- `<outDir>`: The output directory where analysis results will be saved.

## Example Usage
```
./htgts.sh /path/to/directory JT8572_S1_R1_001.fastq JT8572_S1_R2_001.fastq libseqInfo.txt libseqInfo2.txt /path/to/directory/output
```

## Requirements
- Docker must be installed and running on the system.

## Notes
- Ensure that input files are correctly formatted and placed in the specified directory.
- Verify that the Docker image `repbioinfo/htgts_pipeline_lts` is available locally or download it before executing the script.
```

