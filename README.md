# Bloom-Filter
A sequential and parallel (GPU) implementation of Bloom Filter

First download the sample insert.txt and lookups.txt files [here](https://drive.google.com/drive/folders/1UJcZkmYwIChn0KMl9feTpcr6REffXsiL?usp=sharing) (or create your own)

Steps to run sequential (CPU) code

1. `gcc -o seq_bloomfilter -std=c99 seq_bloomfilter.c `
2. `./seq_bloomfilter inserts.txt lookups.txt`

Steps to run parallel (GPU) code

1. `nvcc -o bloomfilter bloomfilter.cu`
2. `./bloomfilter inserts.txt lookups.txt`

Where:
inserts.txt contains the strings to be inserted
lookups.txt contains the strings to be looked up
filenames are just placeholders and can be renamed
