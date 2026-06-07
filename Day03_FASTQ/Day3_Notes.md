# Day 3: FASTQ Files + NGS Basics

## What is FASTQ
- Standard format for raw sequencing data
- 4 lines per read: header, sequence, separator, quality
- Header: @read_name
- Sequence: ACGTACGT... (DNA bases)
- Separator: +
- Quality: IIII!!HH... (ASCII characters representing confidence)

## Quality Scores
- I = Q40 = 99.99% accurate (excellent)
- H = Q39 = excellent
- G = Q38 = very good
- ! = Q0 = 50% accurate (poor)
- Standard threshold: Keep Q30+ (99.9% accurate)

## Illumina Sequencing Workflow
1. DNA fragmentation (150-300 bp pieces)
2. Library preparation (add adapters)
3. Cluster generation (amplify 1000x for signal)
4. Sequencing by synthesis (add bases one-by-one, record colors)
5. Base calling (convert colors to ACGT letters)

## Files Created
- sample1.fastq: 5 reads with mixed quality
- sample2.fastq: 3 reads simulated real data
- combined.fastq: 8 reads total merged

## Commands Learned
- grep -c '^@': Count reads
- awk 'NR%4==2': Extract sequences
- awk 'NR%4==0': Extract quality
- cat file1 file2 > combined: Merge files

