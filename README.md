#PBS -S /bin/bash
#PBS -N rnaspades
#PBS -j oe
#PBS -o rnaspades.log
#PBS -l nodes=genom.local:ppn=30
#PBS -d /gpfs_bkp/HOME/aaksenova/paradaedalea/rnaspades


python /gpfs_bkp/HOME/aaksenova/SPAdes-3.12.0/bin/spades.py --rna -1 ../paradaedalea_non_rRNA_R1.fastq -2 ../paradaedalea_non_rRNA_R2.fastq -t 30 -o ./
# rnaSpades
