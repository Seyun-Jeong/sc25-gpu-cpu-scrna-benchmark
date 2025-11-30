# SC25 GPU-CPU scRNA-seq Benchmark

Paper materials for "Evaluating Accuracy and Performance Tradeoffs in GPU Accelerated Single Cell RNA-seq Analysis"

SC Workshops '25 — Best Paper Runner-Up

DOI: https://doi.org/10.1145/3731599.3767378

## Summary

We ran the same scRNA-seq pipeline (preprocessing, PCA, clustering) on 1.3M mouse brain cells using both Scanpy (CPU) and RAPIDS (GPU). The clustering results only moderately agreed (ARI ≈ 0.5), even though the algorithms are supposed to be equivalent.

This matters because the same patient data, processed by the same algorithm, can yield different clusters depending on hardware.

## Authors

Gardner, Jeong, Khatavkar, Moon, Cao, Ahn — Saint Louis University


## Tools

Benchmarked existing pipelines:
- CPU: Scanpy 1.9 (https://scanpy.readthedocs.io/)
- GPU: RAPIDS single-cell examples (https://github.com/NVIDIA-Genomics-Research/rapids-single-cell-examples)

## Environment

- Python 3.10
- Scanpy 1.9
- RAPIDS 24.02
- NVIDIA H100 (80GB)
- Intel Xeon 6548Y (64 cores)

## Data

10x Genomics 1.3M Mouse Brain Cells:
https://www.10xgenomics.com/datasets/1-3-million-brain-cells-from-e-18-mice-2-standard-1-3-0

## Code

Benchmark scripts are maintained by the BioHPC Lab. Contact the corresponding author for access.

## Citation

Gardner, Jeong, et al. "Evaluating Accuracy and Performance Tradeoffs in GPU Accelerated Single Cell RNA-seq Analysis." SC Workshops '25.
https://doi.org/10.1145/3731599.3767378
