# Hebbian learning

↑ **Parent:** [Unsupervised learning](unsupervised-learning.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hebbian_learning)

Activity-dependent strengthening associated with coactivation of an input and its postsynaptic output. The idealized update $\Delta w_i\propto yx_i$ requires normalization, competition or other constraints to prevent indefinite weight growth.

In [Hebbian memory weights for a Hopfield network](hebbian-memory-weights-for-a-hopfield-network.md), the local update $\Delta w_{ij}=\eta\xi_i\xi_j$ records a pairwise association, where $\eta>0$ and $\xi_i,\xi_j\in\{-1,1\}$. Equal signs strengthen a positive coupling; opposite signs favor a negative coupling. Summing such updates gives a [symmetric matrix](symmetric-matrix.md) of pairwise associations. This is a storage prescription: it does not by itself compare the generated [probability distribution](probability-distribution-split.md) with the [training data](training-data.md), as [Boltzmann machine](boltzmann-machine.md) learning does. Bipolar activity also makes joint inactivity contribute positively; this encoding is a mathematical idealization, not a literal statement about inactive biological cells.

**Table of contents**

- [Quartic norm stabilization of Hebbian learning](quartic-norm-stabilization-of-hebbian-learning.md)
- [Oja's rule](oja-s-rule.md)
  - [Stability and normalization of averaged Oja learning](stability-and-normalization-of-averaged-oja-learning.md)

## ↑ Ancestors (8)

1. [Unsupervised learning](unsupervised-learning.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Activity-dependent ocular dominance segregation](activity-dependent-ocular-dominance-segregation.md)
- [Correlation-based development of visual cortical maps](correlation-based-development-of-visual-cortical-maps.md)
- [Orientation-map self-organization](orientation-map-self-organization.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/6e/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/6e/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/6e/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/3/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73/4/e/solution.md)
- [Quartic norm stabilization of Hebbian learning](quartic-norm-stabilization-of-hebbian-learning.md)
- [Synaptic normalization](synaptic-normalization.md)
