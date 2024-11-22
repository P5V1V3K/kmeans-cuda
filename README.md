# K-means parallel computing in CUDA

## How to run this code

Before trying to execute both sequential and parallel version of k-means algorithm it is important to extract `datapoints.zip` in the same folder of the codes.

The parameters will be initialized according to user choices after the execution start.

If you want to visualize the results you need to create in the same folder of the code a directory named `outdir`, execute your simulation and then take the file `clusters.csv` from `outdir`, which 
must be used in the python script `cluster_displayer.py`.

1. sequential compiler line on linux:
    ```terminal
    g++ -o kmeans_sequential kmeans_sequential.cpp
    ```

2. parallel compiler line on linux:
    ```terminal
    nvcc kmeans_parallel.cu -o kmeans_parallel
    ```
