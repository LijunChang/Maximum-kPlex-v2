# Maximum k-Plex Computation: Theory and Practice

This repository implements the maximum k-plex computation algorithm kPlexT proposed in our SIGMOD 2024 paper. If you are using the code, please cite our paper.
<pre>
Lijun Chang:
Maximum k-Plex Computation: Theory and Practice.
Proc. ACM Manag. Data 2(1): 63:1-63:26 (2024)
</pre>

This repository is the same as https://github.com/LijunChang/Maximum-kPlex-v2

## Compile the code

```sh
$ make clean
$ make
```
It generates an executable "kPlexT", which corresponds to the kPlexT algorithm.

## Run the code

```sh
$ ./kPlexT -g {path_to_graph} -k {k_value}
```

An example of computing the exact maximum 3-plex for the dataset CA-GrQc is as follows
```sh
$ ./kPlexT -g datasets/CA-GrQc -k 3
```

## Data format
Two data formats are supported. The default data format is "edges.txt", which contains a list of undirected edges represented as vertex pairs. The first line contains two numbers n and m, representing the number of vertices and the number of undirected edges, respectively. Note that, the vertex ids must be between 0 and n-1.

## Get datasets
10th DIMACS graphs collection: https://networkrepository.com/dimacs10.php

Real-world graphs collection: http://lcs.ios.ac.cn/~caisw/Resource/realworld%20graphs.tar.gz
