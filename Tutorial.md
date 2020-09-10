This program identifies unknown lineages of Phytophthora infestans based on 12 commonly used SSR markers (microsatellite data). 

How it works

The SSRMatcher compares the SSR data for your isolates of interest to over 2,500 described isolates in our database. The closest genetic match is determined using Bruvo’s distance (described [here](https://doi.org/10.1111/j.1365-294x.2004.02209.x)).

How to collect data for this program

This program uses results obtained from a 12-plex microsatellite amplification for Phytophthora infestans. These 12 microsatellite loci are well described for Phytophthora infestans and vary across lineages, allowing identification of different genotypes of the pathogen. Genotyping using this method first involves running the microsatellites to allelic data for each loci, which is described [here](https://doi.org/10.1016/j.mimet.2012.11.021). 

The raw microsatellite reads obtained from that methodology must then be processed and scored to create input data for the SSR Matcher. This data will be available as a trace file (.fsa), which will contain colored peaks corresponding to lengths of different genetic fragments. The 12-plex protocol described at the link above uses five dyes and generates thirteen series of fragments in total. The 12 microsatellite loci are represented by four different dye colors, with fragment length between those with like colors dissimilar enough to allow for differentiation. There is also a ladder included, which will have its own color of dye. The raw reads visible in this trace file can be scored using several different bioinformatics programs, including Geneious, a popular paid program, and STRand, a free resource provided by UC Davis. Using one of these programs or something similar, the researcher identifies the peak (or peaks if heterozygous) of fluorescence for a particular color in a particular region. Using the tables below, this dye color and fragment length combination can be used to identify different alleles. Once the alleles are determined from the peak data, they can be formatted similar to the (EXAMPLE CSV) and uploaded to this tool for genotype identification. 

How to upload data
Upload a CSV file containing metadata about your sample as well as SSR data for the 12 loci of interest. Follow the format in the example CSV. We recommend downloading this CSV, replacing the data with your own, and re-uploading it. The matcher will still work if your data is missing some loci, but at least 10 loci are recommended for the most accurate results. Include as many samples as you want. 

How to interpret results
If a close match is found for your sample, the program will return information about the match from our database. This will include a genotype identification (if available) as well as a short statement about the genotype. Additional metadata specific to the sample will also be provided. For example, if the sample you provide is most similar to a US_1 isolate found specifically in China, this location data will be returned. It is hoped that this additional metadata might provide helpful insight into the sample you are studying. 

Having issues?
If you are unable to upload your samples and run the SSRMatcher, please email the CSV file you are using and the problem occurring to acoombe@ncsu.edu.
