## Description of supplementary datasets

### Dataset S1 — dataset for per-sample features
| Category | Description |
| --- | --- |
| fieldsample_barcode | Sequenced sample identifier |
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
| ENA_ID | Sample identifier in [ENA](https://www.ebi.ac.uk/ena/browser) |
| ENA_raw1 | ENA identifier for batch 1 of raw Nanopore signal data |
| ENA_raw2 | ENA identifier for batch 2 of raw Nanopore signal data |
| ENA_raw3 | ENA identifier for batch 3 of raw Nanopore signal data |
| ENA_reads | ENA identifier for the sequenced reads |
| ENA_assembly | ENA identifier for the metagenomic assemblies |

### Dataset S2 — dataset for shallow metagenomes used for multi-sample binning
| Category | Description |
| --- | --- |
| MFD-LR | MFD sample that was deeply sequenced with Nanopore |
| MFD-SR | MFD sample (shallow metagenome) that was used for multi-sample binning |

### Dataset S3 — dataset for per-MAG features
| Category | Description |
| --- | --- |
| fieldsample_barcode | Sequenced sample identifier |
| bin | Genome bin iidentifier |
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
| drep_cluster | Genome bin de-replication cluster identifier |
| rep_status | Genome bin status as species representative within the de-replicated bins |
| ENA_ID | ENA identifier for the genome bin (representative bins only) |
| GTDB_taxonomy | MAG taxonomic classification, reported by GTDB-tk |
| GTDB_REF | Reference genome identifier for species level matches |
| GTDB_ANI | Average nucleotide identity for a top match, reported by GTDB-tk |
| GTDB_AF | Alignment fraction for tpå match, reported by GTDB-tk |
| GTDB_MSA | Percentage of amino acids in the multi-sequence alignment, reported by GTDB-tk |
| GTDB_RED | Relative Evolutionary Divergence for a distant match, reported by GTDB-tk |
| SILVA_taxonomy | MAG 16S rRNA taxonomic classification to the SILVA database (top hit) |
| SILVA_identity | Identity of the MAG 16S rRNA to the top hit match in SILVA |
| SILVA_length | Alignment length between the MAG 16S rRNA and SILVA sequence |

### Dataset S4 — DRAM annotation results for Oederibacterium danicum genome
 Category | Description |
| --- | --- |
| gene_id | Unique identifier for each gene in the annotation results |
| fasta | Name of the file from which the gene was annotated |
| scaffold | Identifier for the scaffold or contig where the gene is located |
| gene_position | Position of the gene within the scaffold |
| start_position | Start coordinate of the gene |
| end_position | End coordinate of the gene |
| strandedness | Orientation of the gene |
| rank | Rank of the gene based on annotation confidence or completeness |
| kegg_genes_id | KEGG database identifier for the matched gene |
| ko_id | KEGG Orthology (KO) identifier assigned to the gene |
| kegg_hit | Description of the best KEGG database match |
| kegg_RBH | Indicates whether the KEGG match was a reciprocal best hit (RBH) |
| kegg_identity | Percent identity of the gene to the KEGG database match |
| kegg_bitScore | Bit score of the KEGG database match |
| kegg_eVal | E-value of the KEGG database match |
| peptidase_id | Identifier for the peptidase match from the MEROPS database. |
| peptidase_family| Peptidase family classification according to the MEROPS database |
| peptidase_hit | Description of the best peptidase match |
| peptidase_RBH | Indicates whether the peptidase match was a reciprocal best hit |
| peptidase_identity | Percent identity of the gene to the peptidase database match |
| peptidase_bitScore | Bit score of the peptidase database match |
| peptidase_eVal | E-value of the peptidase database match |
| pfam_hits | List of Pfam protein domain annotations associated with the gene. |
| cazy_ids | CAZy database identifiers assigned to the gene |
| cazy_hits | Description of the best CAZy match |
| cazy_subfam_ec | CAZy subfamily and enzyme classification (EC number) |
| cazy_best_hit | Best-scoring CAZy annotation for the gene |
| heme_regulatory_motif_count | Number of heme regulatory motifs detected in the gene sequence |

### Dataset S5 — dataset for proposing novel lineages under SeqCode
| Category | Description |
| --- | --- |
| bin | Genome bin identifier |
| genus_type | Status of the genome as nomenclatural type for the genus |
| genus_proposed | Proposed genus name for lineage |
| species_proposed | Proposed species name for lineage |
| language | Language of the proposed name (N.L. — Neo Latin) |
| gender | Grammatical gender of the lineage name |
| genus_explanation | Explanation of the genus name |
| species_explanation | Explanation of the species name |
| genus_status| Status of the genome at genus-level taxonomy |
| species_status | Status of the genome at species-level taxonomy |
| novelty_method | Method used to determine novelty of the genome |
| accession | ENA identifier for the genome bin |
| sequencing_technology | Name of the sequencing platform used to sequence the genome |
| binning_workflow | Name of the bioinformatics workflow used to recover the genome |
| genome_size | Size of the genome in bp |
| total_contigs | Number of contigs for the genome |
| coverage | Average genome bin coverage, reported by CoverM |
| GC_content | Genome bin guanine-cytosine content percentage |
| completeness_estimate | Genome bin completeness estimate, reported by CheckM2 |
| contamination_estimate | Genome bin contamination estimate, reported by CheckM2 |
| count_16S | Number of detected 16S rRNA genes |
| count_tRNA | Number of detected different tRNA genes |
| taxonomy_GTDB | MAG taxonomic classification, reported by GTDB-tk |
| taxonomy_SILVA | MAG 16S rRNA taxonomic classification to the SILVA 138.2 database (top hit) |
| taxonomy_SILVA_perc | Identity of the MAG 16S rRNA to the top hit match in SILVA |
| sample_name | Sequenced sample identifier |
| sample_country | Country of origin for the sequenced sample |
| longitude | Sample longitude coordinates |
| latitude| Sample latitude coordinates |
| sample_type | Sample type |
| sample_habitat_broad | Broad-scale environmental context (same as mfd_hab1) |
| sample_habitat_local | Local environmental context (mfd_hab3 or mfd_hab2, if mfd_hab3 missing) |

[//]: # (Written by Mantas Sereika)
