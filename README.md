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
  	
  1.[Trimmomatic](http://www.usadellab.org/cms/uploads/supplementary/Trimmomatic/Trimmomatic-Src-0.38.zip)  
  2.[bwa](https://sourceforge.net/projects/bio-bwa/files/bwa-0.7.17.tar.bz2/download)  
  3.[samtools](https://sourceforge.net/projects/samtools/files/latest/download)  
  4.[picard](https://github.com/broadinstitute/picard/releases/download/2.18.15/picard.jar)    
  5.[GATK](https://github.com/broadinstitute/gatk/releases/download/4.0.11.0/gatk-4.0.11.0.zip)   
  6.[VEP](https://github.com/Ensembl/ensembl-vep/archive/release/94.zip)
  7.[JAVA]   
  8.[Python]   
  9.[Perl]   
  
1-6 tools are better put in the folder Tools/.   

## Installation of each module

1.Trimmomatic   

	unzip Trimmomatic-*.zip

2.bwa

	tar -xjvf bwa-*.tar.bz2
	cd bwa-*
	make

3.samtools
	
	sudo apt-get install libncurses5-dev
	sudo apt-get install libbz2-dev
	sudo apt-get install liblzma-dev
	tar -xjvf samtools-*.tar.bz2
	cd samtools-*
	./configure
	make
	make install

4.GATK

	unzip gatk-*.zip
	sudo apt install openjdk-8-jdk-headless
	
5.VEP

	unzip ensembl-vep-release-*.zip
	perl INSTALL.pl

	
	
