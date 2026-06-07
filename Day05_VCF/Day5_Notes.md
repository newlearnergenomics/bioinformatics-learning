# Day 5: VCF Files + Variants

## What is a Variant
- Difference from reference genome
- Types: SNP (A→T), insertion (add bases), deletion (remove bases)

## VCF Format
- Columns: CHROM, POS, ID, REF, ALT, QUAL, FILTER, INFO
- CHROM: Chromosome (chr1, chr2)
- POS: Position
- REF: Reference allele (what genome has)
- ALT: Alternate allele (what we found)
- QUAL: Quality score (higher=better)
- FILTER: PASS/FAIL
- INFO: Extra data (DP=depth, AF=frequency)

## Variant Calling Workflow
1. Align reads to reference (BAM)
2. Run mpileup (get reads at each position)
3. Call variants (find differences)
4. Filter variants (keep high quality)
5. Output: VCF file

## Variant Types
- SNP: One base change
- Insertion: Bases added
- Deletion: Bases removed
- Indel: Complex change

## Variant Calling Tools
- Samtools/BCFtools: Simple
- GATK: Gold standard
- DeepVariant: AI-based

## Quality Filtering
- Keep: QUAL > 20
- Keep: FILTER = PASS
- Keep: DP > 10
- Remove: Low confidence

## Commands
- bcftools call: Call variants
- bcftools filter: Filter variants
- bcftools stats: Variant statistics

## Complete NGS Pipeline
FASTQ → [Align] → BAM → [Call variants] → VCF → [Filter] → VCF_FILTERED
