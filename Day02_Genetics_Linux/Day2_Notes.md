\# Day 2: June 1-4, 2026 --- Mutations + Genome + Linux Basics

\## Biology Learned

\### Mutations (Amoeba Sisters)

\- \*\*What is a mutation?\*\* A change in DNA sequence

\- \*\*Types of mutations:\*\*

\- Point mutation: One base changes (A→G)

\- Insertion: New bases added

\- Deletion: Bases removed

\- \*\*Impact:\*\* Can be good (evolution), bad (disease), or neutral (no effect)

\- \*\*Most mutations don\'t cause problems\*\* but some cause serious disease

\### Genome (NHGRI)

\- \*\*Definition:\*\* Complete set of DNA instructions in an organism

\- \*\*Human genome size:\*\* 3.2 billion base pairs

\- \*\*Contains:\*\* \~20,000 genes

\- \*\*Information:\*\* All instructions to build and maintain a person

\- \*\*Location:\*\* Nucleus of every cell (mostly)

\- \*\*Why it matters:\*\* Understanding genomes = understanding disease, evolution, personalized medicine

\## Linux Commands Learned

\### Basic Commands

\| Command \| What it does \| Example \|

\|\-\-\-\-\-\-\-\--\|\-\-\-\-\-\-\-\-\-\-\-\--\|\-\-\-\-\-\-\-\--\|

\| \`cat\` \| View file content \| \`cat genes.txt\` \|

\| \`wc -l\` \| Count lines \| \`wc -l genes.txt\` \|

\| \`grep\` \| Search for text \| \`grep \"cancer\" genes.txt\` \|

\| \`grep -c\` \| Count matches \| \`grep -c \"cancer\" genes.txt\` \|

\| \`cut -f\` \| Extract columns \| \`cut -f1 genes.txt\` \|

\### Pipes (\|) --- The Game Changer

A pipe \`\|\` means: \"Take output from first command, send to second command\"

\*\*Examples:\*\*\
grep \"cancer\" genes.txt \| wc -l → Find cancer lines, then count them = 5

cut -f2 genes.txt \| sort → Extract disease column, then sort alphabetically

grep \"cancer\" genes.txt \| cut -f1 \| sort → Find cancer genes, extract names, sort them

\## Practice Data Created

\### genes.txt

\- 7 genes with associated disease and risk level

\- Used to practice: grep, cut, wc, pipes

\- Real bioinformatics data structure

\### expression.txt

\- Gene expression levels in tumor vs normal cells

\- 5 genes with status (overexpressed, underexpressed, normal)

\- Used to practice filtering and combining commands

\## Key Concepts Understood

✓ Mutations are changes in DNA

✓ Genome = complete DNA blueprint

✓ grep = search in files

✓ cut = extract specific columns

✓ Pipes = connect commands together

✓ Can combine 2-3+ commands with pipes

\## Confidence Level

\- Biology (mutations): 8/10

\- Biology (genome): 8/10

\- Linux basics: 7/10

\- Pipes: 8/10

\- grep + cut: 8/10

\## What\'s Next

\- FASTQ file format (real sequencing data)

\- Quality control of sequences

\- Alignment concepts

\- Real bioinformatics workflows

\## Notes

\- Taking things slow helps understanding

\- Pipes are the most powerful concept

\- Practice commands multiple times for muscle memory

\- Real learning happens when working with actual data

\-\--

Created: June 1-4, 2026

Status: Day 2 Complete ✓

EOF
