# Euplotes vannus genomic analysis
Perl scripts used in Euplotes vannus genomic data analysis

----------------------------------------
## 1. Coverage distribution of scaffolds
### 01scf_coverage_distribution.pl

Usage:

    perl 01scf_coverage_distribution.pl  Str.sul_scaffolds_nobac_nomito_noredundancy.fasta

----------------------------------------
## 2. Filter out low coverage scaffolds
### 02scf_coverage_selection.pl

Usage:

    perl 02scf_coverage_selection.pl  <genome file>  <coverage_cutoff>  <scaffold_length_cutoff>

----------------------------------------
## 3. Separate scaffold into different groups based on telomeres' presence
### 03scf_telomere_selection.pl

Usage:

    perl 03scf_telomere_selection.pl  <genome file>  <output_dir>

----------------------------------------
## 4. Split fragments in SAM file into mapped and unmapped after mapping
### 04split_sam_into_mapped_unmapped.pl

Usage:

    perl split_sam_into_mapped_unmapped.pl <SAM file>

----------------------------------------
## 5. List names of mapped contigs/scaffolds in SAM file
### 05list_sam_mapped_targets.pl

Usage:

    perl 05list_sam_mapped_targets.pl <SAM file>

----------------------------------------
## 6. Filter out genes without RNA-seq reads mapping
### 06validation_gene_prediction_byRNAseq.pl

Usage:

    perl 06validation_gene_prediction_byRNAseq.pl  <Gene data file>  <RNA-seq mapping list>  <Output file>

----------------------------------------
## 7. Detect frameshifting events from output file of BLASTX
### 07frameshifting_detect_BLASTX_tab.pl

Usage:

    perl 07frameshifting_detect_BLASTX_tab.pl  <input_file BLASTX tab>  <output file1 frameshifting BLASTX tab>  <output file2 frameshifting adjacent region>  <frame_distance>
