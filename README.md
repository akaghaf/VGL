# VGL

The purpose of this project is to create a tool that automates the creation of visuals and variant optimization.
After generating these prioritized variants files  the investigator needs to digest all the data which includes combining data sets and generating list of SNPs for further evaluation. The pipeline was created by Dr. Brad Till in 2022 and the scripts can be found on the VGL Github page VCF_Subsetting_Tools_Local 
The SOP by undergraduate intern Hannah Echt, Dr. Bellone , and Dr. Till on 8_26_2022 and the final version (1) was approved for use on 9/7/22 by Dr. Bellone.  
The variant callers use different algorithms to identify nucleotide changes, attempting to strike a balance between sensitivity (finding all possible variation, avoiding false negative errors) and reducing false positive errors (cases where the tool predicts a variant that isn’t real).  Thus, the highest confidence variants are those that are identified by all three variant callers and are predicted by SNPeff to affect gene function.   

In the same directory the program is being ran in, there must be 6 directories named as they appear in the repository, and within them 1 file each, named respectively. Also in the same directory as the program would be a "samples.txt". This is similar to the samples file that is input into the pipeline created by Dr. Till. The first column denotes sample names, the second column consists of sample genotype codes, and the third column denotes "c" for case and "n" for control.
