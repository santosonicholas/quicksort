# SEQUENTIAL QUICKSORT AND PARALLEL QUICKSORT

This is a comparison between sequential quicksort and parallel quicksort

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
GCC
```

### Installing

```
1. Download quicksort.c and quicksort_parallel.c
2. Make the file can compile with type in the terminal (must in the directory path) 
"g++ quicksort.c -o quicksort -fopenmp" or ""g++ quicksort_parallel.c -o quicksort_parallel -fopenmp -fpermissive"
3. Execute the file with type in the terminal (must in the directory path) "./quicksort (samplesize).txt
```

## Running the tests

Test is done with both sequential and parallel quicksort programs to find the average time taken to finish quicksorting with a sample size of 10, 100, 1000 and 10000.

### Sequential Quicksort

|Sample Size|Test 1      |Test 2      |Test 3      |Average Time|
|-----------|------------|------------|------------|------------|
|10         |0.000000 sec|0.000001 sec|0.000001 sec|0.000001 sec|
|100        |0.000010 sec|0.000043 sec|0.000010 sec|0.000021 sec|
|1000       |0.000543 sec|0.000504 sec|0.000480 sec|0.000509 sec|
|10000      |0.031954 sec|0.034133 sec|0.032917 sec|0.033001 sec|

### Parallel Quicksort

|Sample Size|Test 1       |Test 2       |Test 3       |Average Time   |
|-----------|-------------|-------------|-------------|---------------|
|10         |0.0010540 sec|0.0013190 sec|0.0013110 sec|0.001228000 sec|
|100        |0.0078230 sec|0.0080990 sec|0.0096210 sec|0.008514333 sec|
|1000       |0.3001000 sec|0.3200510 sec|0.3348290 sec|0.318326667 sec|
|10000      |13.148478 sec|16.086526 sec|13.648602 sec|14.29453533 sec|

## Result
Test is done with finding the average time with quicksorting sequentially and parallel with a sample size of 10, 100, 1000, and 10000

### Singular Quicksort vs Parallel Quicksort Time Comparison

|Sample Size|Sequential  |Parallel       |
|-----------|------------|---------------|
|10         |0.000001 sec|0.001228000 sec|
|100        |0.000021 sec|0.008514333 sec|
|1000       |0.000509 sec|0.318326667 sec|
|10000      |0.033001 sec|14.29453533 sec|


### Graph Time Comparison

![Graph](https://github.com/santosonicholas/quicksort/blob/master/chartSequentialParallelQuickSort.PNG)

### Result Analysis
From the result we can see that sequential quicksort is much faster than parallel quicksort. Because in the parallel quicksort must do parallelism job, thread creation, time for synchronization, etc. And sequential quicksort just sorting normally with the following algorithm and do not care about the parallelism.

## Authors

* Nicholas - UPH Informatics 2017

## License

This project is licensed under the MIT License

## Acknowledgments

* Quicksort Program --> [markwkm](https://github.com/markwkm/quicksort)
* Guidebook Quicksort Algorithm --> [Tinku Singh & Durgesh Kumar Srivastava](https://pdfs.semanticscholar.org/cba9/770c4fad941fe5e501539525953a242a36f8.pdf)
* Template README.md --> [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
