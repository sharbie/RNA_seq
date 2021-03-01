Samtools Installation
Follow general instruction

hisat2
sudo apt update
sudo apt install hisat2

Cufflinks:
Follow all general instuction first.
For boost lib:
sudo apt install libboost1.71-tools-dev

For bam lib:
mkdir -p /usr/local/include/bam
cp ${SAMTOOLS}/libbam.a /usr/local/lib/
cp ${SAMTOOLS}/*.h /usr/local/include/bam
cp ${SAMTOOLS}/samtools /usr/local/bin/
rename XXX/include/bam/version.h to XXX/include/bam/version.hpp

resource: http://linuxtoolkit.blogspot.com/2013/04/unable-to-detect-bamlib-libraries.html
