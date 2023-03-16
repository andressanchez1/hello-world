# hello-world
This is my new and cool repository
Yay :)


fastqc:

fastqc *
fastqc 11_S20_L001_R1_001.fastq.gz
fastqc output_trimmed_11_S20_L001_R1_001_paired2.fastq.gz

Trimmomatic:
Pair-end

trimmomatic PE 11_S20_L001_R1_001.fastq.gz 11_S20_L001_R2_001.fastq.gz  output_trimmed_11_S20_L001_R1_001_paired.fastq.gz output_trimmed_11_S20_L001_R1_001_unpaired.fastq.gz output_trimmed_11_S20_L001_R2_001.fastq_paired.fastq.gz output_trimmed_11_S20_L001_R2_001_unpaired.fastq.gz ILLUMINACLIP:TruSeq3-PE-2.fa:2:30:10:2:keepBothReads LEADING:3 TRAILING:3 CROP:200 MINLEN:36


SE
trimmomatic SE 11_S20_L001_R1_001.fastq.gz output_trimmed_11_S20_L001_R1_001_paired2.fastq.gz  ILLUMINACLIP:TruSeq3-SE-3.fa:2:35:10:2:keepBothReads LEADING:3 TRAILING:5 CROP:200 MINLEN:36
