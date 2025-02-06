## Description of supplementary datasets

### Dataset S1 — dataset for per-sample features
| Category | Description |
| --- | --- |
| fieldsample_barcode | Sequenced sample ID |
| habitat_typenumber | Sample habitat type number, as described in the [MFD metadata](https://github.com/cmc-aau/mfd_metadata) |
| mfd_sampletype | Sample type |
| mfd_areatype | Sample area type |
| mfd_hab1 | Sample habitat descriptor (level 1) |
| mfd_hab2 | Sample habitat descriptor (level 2) |
| mfd_hab3 | Sample habitat descriptor (level 3) |
| longitude | Sample longitude coordinates |
| latitude | Sample latitude coordinates  |
| assembled | Percentage of sequenced reads that mapped to the assembly, reported by Flye |
| reads_n | Number of sequenced reads, reported by Nanoq |
| reads_size_bp | Sequenced read yield in bp, reported by Nanoq |
| reads_N50_bp | Sequenced read N50 in bp, reported by Nanoq |
| reads_len_max_bp | Length of the longest sequenced read in bp, reported by Nanoq |
| reads_len_min_bp | Length of the shortest sequenced read in bp, reported by Nanoq |
| reads_mean_len_bp | Mean sequenced read length in bp, reported by Nanoq |
| reads_median_len_bp | Median sequenced read length in bp, reported by Nanoq |
| reads_mean_q | Mean sequenced read Phred quality score, reported by Nanoq |
| reads_median_q | Median sequenced read Phred quality score, reported by Nanoq |
| contigs_n | Number of contigs, reported by Nanoq |
| contigs_size_bp | Metagenome size in bp, reported by Nanoq |
| contigs_N50_bp | Metagenomic contig N50 value in bp, reported by Nanoq  |
| contigs_len_max_bp | Length of the longest contig in bp, reported by Nanoq |
| contigs_len_min_bp | Length of the shortest contig in bp, reported by Nanoq |
| contigs_mean_len_bp | Mean contig length in bp, reported by Nanoq |
| contigs_median_len_bp | Median contig length in bp, reported by Nanoq |
| HQ_mags | High-quality MAG count |
| MQ_mags | Medium-quality MAG count |
| r_abund | Percentage of sum MAG relative abundance with mapped reads |
| r_abund_hq | Percentage of sum high-quality MAG relative abundance with mapped reads |
| nanopore | Nanopore chemistry used for sequencing |
| speed_bps | Nanopore sequencing speed mode in bps |
| sampling_khz | Nanopore sequencing sampling rate in KHz |
| device | Sequencing device used for sample |
| minknow_v | Version of MinKNOW used during sequencing |
| basecaller | Basecaller name |
| basecaller_v | Basecaller version |
| ENA_ID | Sample ID in [ENA](https://www.ebi.ac.uk/ena/browser) |
| ENA_raw1 | ENA ID for batch 1 of raw Nanopore signal data |
| ENA_raw2 | ENA ID for batch 2 of raw Nanopore signal data |
| ENA_raw3 | ENA ID for batch 3 of raw Nanopore signal data |
| ENA_reads | ENA ID for the sequenced reads |
| ENA_assembly | ENA ID for the metagenomic assemblies |

### Dataset S2 — dataset for shallow metagenomes used for multi-sample binning
| Category | Description |
| --- | --- |
| MFD-LR | MFD sample that was deeply sequenced with Nanopore |
| MFD-SR | MFD sample (shallow metagenome) that was used for multi-sample binning |

### Dataset S3 — dataset for per-MAG features
| Category | Description |
| --- | --- |
| fieldsample_barcode | Sequenced sample ID |
| bin | Genome bin ID |
| Completeness_CheckM1 | Genome bin completeness estimate, reported by CheckM |
| Contamination_CheckM1 | Genome bin contamination estimate, reported by CheckM |
| Strain_Heterogeneity | Genome bin strain heterogeneity estimate, reported by CheckM |
| Completeness_CheckM2 | Genome bin completeness estimate, reported by CheckM2 |
| Contamination_CheckM2 | Genome bin contamination estimate, reported by CheckM2 |
| Coding_Density | Genome bin gene coding density value, reported by CheckM2 |
| Contig_N50 | Genome bin N50 in bp, reported by CheckM2 |
| Average_Gene_Length | Average gene length in bp, reported by CheckM2 |
| Genome_Size | Genome bin size in bp, reported by CheckM2 |
| GC_Content | Genome bin guanine-cytosine content percentage |
| Total_Contigs | Number of contigs, reported by CheckM2 |
| Max_Contig_Length | Length of the longest contig in bp, reported by CheckM2 |
| N90 | Genome bin N90 in bp, reported by Quast |
| auN | Nx area under the curve, reported by Quast |
| N_per_100kb | Rate of Ns in a genome bin per 100 kb, reported by Quast |
| cov | Average genome bin coverage, reported by CoverM |
| r_abund | Average genome bin relative abundance (%), reported by CoverM |
| CDS_all | Number of protein coding genes, reported by Bakta |
| CDS_hyp | Number of hypothetical protein coding genes, reported by Bakta |
| bakta_tRNA_all | Number of all tRNA genes genes, reported by Bakta |
| bakta_tRNA_uniq |  Number of unique tRNA genes genes, reported by Bakta |
| bakta_16S | Number of 16S rRNA genes genes, reported by Bakta |
| bakta_23S | Number of 23S rRNA genes genes, reported by Bakta |
| bakta_5S | Number of 5S rRNA genes genes, reported by Bakta |
| bac_16S | Number of 16S rRNA genes genes, reported by Barrnap (bacterial model) |
| bac_23S | Number of 23S rRNA genes genes, reported by Barrnap (bacterial model) |
| bac_5S |  Number of 5S rRNA genes genes, reported by Barrnap (bacterial model) |
| arc_16S | Number of 16S rRNA genes genes, reported by Barrnap (archaeal model) |
| arc_23S | Number of 23S rRNA genes genes, reported by Barrnap (archaeal model) |
| arc_5S | Number of 5S rRNA genes genes, reported by Barrnap (archaeal model) |
| bac_trna | Number of unique tRNA genes genes, reported by tRNAscan-SE (bacterial model) |
| arc_trna | Number of unique tRNA genes genes, reported by tRNAscan-SE (archaeal model) |
| MAG_status | Genome bin quality ranking according to [MIMAG standards](https://www.nature.com/articles/nbt.3893) |
| MAG_status2 | Genome bin ranking from `MAG_status`, where circular MAGs are marked separately |
| drep_cluster | Genome bin de-replication cluster ID |
| rep_status | Genome bin status as species representative within the de-replicated bins |
| ENA_ID | ENA ID for the genome bin (representative bins only) |
| GTDB_taxonomy | MAG taxonomic classification, reported by GTDB-tk |
| GTDB_REF | Reference genome ID for species level matches |
| GTDB_ANI | Average nucleotide identity for a top match, reported by GTDB-tk |
| GTDB_AF | Alignment fraction for tpå match, reported by GTDB-tk |
| GTDB_MSA | Percentage of amino acids in the multi-sequence alignment, reported by GTDB-tk |
| GTDB_RED | Relative Evolutionary Divergence for a distant match, reported by GTDB-tk |

### Dataset S4 — dataset for proposing novel lineages under SeqCode
| Category | Description |
| --- | --- |
| bin | Genome bin ID |
| genus_proposed | Proposed genus name for lineage |
| species_proposed | Proposed species name for lineage  |
| gender | Grammatical gender of the lineage name |
| genus_explanation | Explanation of the genus name |
| species_explanation | Explanation of the species name |
| GTDB_phylum | Phylum taxononomy of the lineage in GTDB R220 |
| GTDB_class | Class taxononomy of the lineage in GTDB R220 |
| GTDB_order | Order taxononomy of the lineage in GTDB R220 |
| GTDB_family | Family taxononomy of the lineage in GTDB R220 |

[//]: # (Written by Mantas Sereika)
