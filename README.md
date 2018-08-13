# IA-SPGEMM

IA-SPGEMM is a An Input Auto-tuning Sparse General Matrix-Matrix Multiplication on Multicore and Manycore Architure. Currently
supported co include:

- SpGEMM algorithms for COO, DIA and ELL sparse storage formats
- Feature extraction and density representation
- MatNet (mix CNN and BP)

All tests default calculate the square of A for matrix inputs. 

The tool extracts all of the features and density representation as MatNet inputs.

It is easy to use and provide unified interface.

## Getting Started
In IA-SPGEMM system, the goal is to search an optimal format and algorithm that minimizes computing overhead.

Setting up an IA-SPGEMM is easy.

```bash
i.e., ./IA-SPGEMM-CPU_release/spgemm-cpu ./IA-SPGEMM-CPU_release/Inputs/dia.mtx
```

**Intel & AMD CPU example**

<img src="https://github.com/AnonymousPPOPP2019/IA-SPGEMM/blob/master/IA-SPGEMM-CPU_release/1.jpg"/>

**NVIDIA GPU example**

<img src="https://github.com/AnonymousPPOPP2019/IA-SPGEMM/blob/master/IA-SPGEMM-GPU_release/2.jpg"/>

## Requirement
- Intel MKL 2018
- CUSP v0.5.1
- cuSPARSE v8.0
- Python 3.5.2
- tensorflow 1.4.0
- keras 2.1.0

## MatNet
Details of the neural network
<img src="https://github.com/AnonymousPPOPP2019/IA-SPGEMM/blob/master/model.png"/>
<div align=center><img width="150" height="150" src="https://github.com/AnonymousPPOPP2019/IA-SPGEMM/blob/master/model.png"/></div>
