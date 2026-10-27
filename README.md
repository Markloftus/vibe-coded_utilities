# vibe-coded_utilities
Useful neat tools I made playing around with LLMs.

## ChromKmer:
ChromKmer is a fast (<15 mins for a 30Gb file at 8 threads), memory-efficient (<1Gb), multithreaded tool that estimates chromosome copy number directly from FASTQ reads by counting chromosome-specific, single-copy k-mer markers. It normalizes marker counts against the median autosomal signal to identify candidate chromosome gains and losses, including autosomal trisomies and sex-chromosome copy-number changes.
