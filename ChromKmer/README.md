Ever wonder how many chromosomes are in your fastq/fastq.gz file? Look no further. This code will tell you chromosome copy number in a 30Gb fastq.gz file in under 15 mins with 8 threads. The README.md in the zipped folder will tell you how to install and supply the yml file for the conda environment it wants. Here is how to run it:

# Do you have paired end read data?
./chromkmer \
  --fastq sample_R1.fastq.gz \
  --fastq sample_R2.fastq.gz \
  --library human.markers.tsv \
  --threads 8 \
  --output results/sample

# Do you have only one file?
  ./chromkmer --fastq sample.fastq.gz \
  --library human.markers.tsv --threads 8 --output results/sample

# Do you have something that is not human?
You will need to build a new --library of unique kmers found on each of your species chromosomes. So as of right now I am only supporting human chromosome copy numbers. 
