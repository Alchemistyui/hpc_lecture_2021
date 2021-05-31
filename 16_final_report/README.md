# hpc_lecture

## 20M38216 Shen Ruoyue

The results of OpenMP+MPI+SIMD+Cache Blocking are all runed in the **login node** of TSUBAME. For different N, run it for **three time** and choose the best one as the result in `results.txt`.

To check the performance, you can run with:

```
module load cuda/11.2.146 openmpi gcc/8.3.0
mpicxx openmp_mpi_simd_cacheblocking.cpp -fopenmp -O3 -march=native
mpirun -np 1 ./a.out
```

