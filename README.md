# Simulation

List of scripts/commands that needs to be run (in order)


1. generate_coords.py
  "python generate_coords.py /home/hkang/volcano/Simulation/static/TruSightTumor_FPA_Manifest.txt /home/hkang/volcano/Simulation/static/coords.bed" 
2. bedtools getfasta
  "/illumina/thirdparty/bedtools/bedtools2-2.22.1/bin/bedtools getfasta -fi /illumina/scratch/iGenomes/Homo_sapiens/UCSC/hg19/Sequence/WholeGenomeFasta/genome.fa -bed {/path/of/output/bed/file} -fo full_seq.txt –tab"

3. generate_template.py
  "python generate_template.py /home/hkang/volcano/Simulation/static/TruSightTumor_FPA_Manifest.txt /home/hkang/volcano/Simulation/static/ /home/hkang/volcano/Simulation/static/full_seq"

4. generate_indel.py / generate_SNV.py
  "python generate_indel.py /home/hkang/volcano/Simulation/static/TruSightTumor_FPA_Manifest.txt /home/hkang/volcano/Simulation/static/template.txt /home/hkang/volcano/Simulation/ 150 25 insertion"

5. generate_reads.sh
  * Change values accordingly inside script

6. combine_reads.sh
  * Change values accordingly inside script
  
7. isis.sh
  * Change values accordingly inside script
