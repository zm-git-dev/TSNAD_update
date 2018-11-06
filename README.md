# TSNAD
 
 Neoantigen prediction from WGS or WES.    
   
 Authors: Zhan Zhou, Jingcheng Wu, Xingzheng Lv.  
 Date: November 2018  
 Version: 1.1  
 License: TSNAD is released under GNU license  

## Introduction  

An integrated software for cancer somatic mutation and tumour-specific neoantigen detection.  

## Requirements
TSNAD uses the following software and libraries:  
  	
1. [Trimmomatic](http://www.usadellab.org/cms/uploads/supplementary/Trimmomatic/Trimmomatic-Src-0.38.zip)  
2. [bwa](https://sourceforge.net/projects/bio-bwa/files/bwa-0.7.17.tar.bz2/download)  
3. [samtools](https://sourceforge.net/projects/samtools/files/latest/download)  
4. [picard](https://github.com/broadinstitute/picard/releases/download/2.18.15/picard.jar)    
5. [GATK](https://github.com/broadinstitute/gatk/releases/download/4.0.11.0/gatk-4.0.11.0.zip)   
6. [VEP](https://github.com/Ensembl/ensembl-vep/archive/release/94.zip)   
7. JAVA     
8. Python    
9. Perl   
  
1-6 tools are better put in the folder Tools/.   

## Installation of each module
1. Trimmomatic   

	unzip Trimmomatic-*.zip

2. bwa

	tar -xjvf bwa-*.tar.bz2
	cd bwa-*
	make

3. samtools
	
	sudo apt-get install libncurses5-dev
	sudo apt-get install libbz2-dev
	sudo apt-get install liblzma-dev
	tar -xjvf samtools-*.tar.bz2
	cd samtools-*
	./configure
	make
	make install

4. GATK

	unzip gatk-*.zip
	sudo apt install openjdk-8-jdk-headless
	
5. VEP

	unzip ensembl-vep-release-*.zip
	perl INSTALL.pl

## Usage

configure the file *somatic_mutation_sequencing_parameters.config* ,

then 

	python  somatic_mutation_sequencing_pipeline.py

configure the file *antigen_predicting_parameters.config* ,

then 

	python antigen_predicting_pipeline.py

## update log

### V1.0 
1. GUI for neoantigen prediction  
2. Two parts: one for somatic mutation detection, another for HLA-peptide prediction.

### V1.1
1. Trimmomatic v0.35 -> v0.38  
2. BWA v0.7.12 -> v0.7.17  
3. Samtools v1.3 -> v1.9  
4. Picard v1.140 -> v2.18.14  
5. GATK v3.5 -> v4.0.8.1  
6. Annovar -> VEP v94  
 

  
 
