# computer-science-basic
This repo contains my notes about the basic concepts of computer science. There are heaps of concepts around computing and sometimes those concepts can be confusing to understand. Two concepts might look very similar to each other. So I am trying to clarify on tiny details that distinguish the concepts. 

This repository is structured into multiple folders that contain a README file inside. Each folder is named with the concept to revise upon. Probably a Github Wiki is a better tool to do this but I am sticking with this first to avoid complexity of deciding which is the best.


## Serialization / Deserialization
- Serialization is converting an object (in programming language) into byte string.
- this string can then be saved in in a file on a harddisk or transmitted over HTTP.
- Deserialization is constructing an object (in programming language) from a series of byte strings.

## Encoding / Decoding
- Encode converts string into byte
	- a = 'test'
	- encoded_a = 'test'.encode('utf8')
- Decode converts byte into string
	- b = b'test'
	- decoded_b = 'test'.decode('utf8')
- ASCII is example of 7-bit byte
- UTF-8 is example of 8-bit byte

## Difference between text file and binary file
- Similarity:
	- both text and binary file contains data based on series of bit
- Difference:
	- different in the way to interpret those bits
- Reference:
	- https://fileinfo.com/help/binary_vs_text_files



## Archive and Compression

## gz vs bz vs xz vs lzma
- ReferenceL
  - https://www.rootusers.com/gzip-vs-bzip2-vs-xz-performance-comparison/

## What is tar
- originally stands for tape archiver based on tape drive storage


# Cryptography

## How encryption works

## Types of encryption

## Network vs Harddisk vs Memory vs CPU Cache speed
