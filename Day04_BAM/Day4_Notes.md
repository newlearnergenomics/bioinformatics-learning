# Day 4: BAM Files + Alignment

## What is Alignment
- Takes reads from FASTQ
- Finds where each read belongs in reference genome
- Output: SAM/BAM file with positions

## SAM Format
- Text, human-readable
- Columns: QNAME, FLAG, RNAME, POS, MAPQ, CIGAR
- QNAME: Read name
- RNAME: Chromosome (chr1, chr2)
- POS: Position in chromosome
- MAPQ: Mapping quality (0-60)
- FLAG: 0=mapped, 4=unmapped, 16=reverse

## BAM Format
- Binary version of SAM
- 4x smaller, faster to process
- Always indexed (.bam.bai)

## Samtools Commands
- samtools view: View alignments
- samtools flagstat: Statistics
- samtools view -F 4: Mapped reads only
- samtools view -f 4: Unmapped only
- samtools depth: Coverage per position
- samtools index: Create index

## Alignment Tools
- BWA: Short reads (100-150 bp)
- STAR: RNA-seq
- Bowtie2: General

## MAPQ Interpretation
- 60: Excellent
- 40-59: Very good
- 20-39: Good
- 10-19: Questionable
- <10: Poor
