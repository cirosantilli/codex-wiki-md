# Hopfield network

↑ **Parent:** [Neural network](neural-network.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hopfield_network)

A recurrent network with symmetric interactions and an energy function. In the binary version, units take values $\pm1$, self-couplings are zero, and asynchronous threshold updates can retrieve stored patterns from incomplete or corrupted cues. Fixed points are local energy minima, which need not be the intended memories or global minima.

For a [symmetric matrix](symmetric-matrix.md) of couplings $W$ with $w_{ii}=0$, define the [energy landscape](energy-landscape.md)

$$
E(x)=-\frac12\sum_{i,j}w_{ij}x_ix_j+\sum_i\theta_ix_i,\qquad x_i\in\{-1,1\}.
$$

The factor $1/2$ removes double counting. The local input is $h_k=\sum_{j\ne k}w_{kj}x_j-\theta_k$. Choosing $x_k$ to agree with $h_k$ lowers this [energy](energy-split.md); this mathematical [energy](energy-split.md) need not be a conserved physical quantity. Its pairwise form connects the model to the [Ising model](ising-model.md); competing couplings also motivate the comparison with a [spin glass](spin-glass.md). Here retrieval seeks a useful nearby [local minimum](local-minimum.md), so reaching the global minimum is not the goal.

[John Hopfield](john-joseph-hopfield.md)'s 1982 computer study stored random [binary strings](binary-string.md) in [neural networks](neural-network.md) of 30 and 100 units. Couplings were prepared from the stored patterns; asynchronous updates supplied the computational apparatus. Starting at each nominal memory, the readout counted [Hamming distances](hamming-distance.md) after settling as storage load varied. Corrupted starting patterns separately tested recovery. Varying the load and cue damage exposed interference between memories. These simulations supported collective retrieval, not a measurement of biological memory capacity.[1982, pp. 2555–2557, storage Eq. 2, Fig. 2 and corrupted-start tests](neural-networks-and-physical-systems-with-emergent-collective-computational-abilities-by-john-joseph-hopfield.md)

**Table of contents**

- [Asynchronous Hopfield energy descent](asynchronous-hopfield-energy-descent.md)
- [Hebbian memory weights for a Hopfield network](hebbian-memory-weights-for-a-hopfield-network.md)
  - [Hopfield recall from a corrupted cue](hopfield-recall-from-a-corrupted-cue.md)

## ↑ Ancestors (8)

1. [Neural network](neural-network.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Associative memory in neural networks](associative-memory-in-neural-networks.md)
- [Boltzmann machine](boltzmann-machine.md)
- [Energy landscape](energy-landscape.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/3/d/solution.md)
- [Spin glass](spin-glass.md)
- [Three-neuron ring stability](three-neuron-ring-stability.md)
