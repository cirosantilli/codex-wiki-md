# Thermal light

↑ **Parent:** [Photon statistics](photon-statistics.md)

For a single mode in [thermal equilibrium](thermal-equilibrium-split.md), its [quantum harmonic oscillator](quantum-harmonic-oscillator-split.md) energy ladder gives a [geometric distribution](geometric-distribution.md)

$$
p_n=(1-q)q^n,\qquad q=e^{-\hbar\omega/(k_{\rm B}T)},\qquad
\mu=\frac{q}{1-q},\qquad 0<q<1.
$$

Its [probability generating function](probability-generating-function.md) is $F(z)=(1-q)/(1-qz)$. Differentiating twice gives $F''(1)=2q^2/(1-q)^2=2\mu^2$, hence $g^{(2)}(0)=2$. At the chosen mean $\mu=2$, $q=2/3$, $p_0=1/3$, $p_1=2/9$, $p_2=4/27$, and $\operatorname{Var}N=6$. Rare high occupations increase the pair count even though the mean matches the other preparations. The geometric weights also arise from a Gaussian mixture of [coherent states](coherent-state.md).[2005 individual Nobel lecture, pp. 91–92, equations (31)–(38)](one-hundred-years-of-light-quanta-by-roy-jay-glauber.md)

<a id="image-three-original-one-mode-photon-number-models-with-the-same-mean-two-and-different-pair-correlations"></a>
![](photon-number-statistics-comparison.png)

**[Figure 1](#image-three-original-one-mode-photon-number-models-with-the-same-mean-two-and-different-pair-correlations). Three original one-mode photon-number models with the same mean two and different pair correlations**. The bars are calculated probabilities, not measured data. Thermal occupations above fourteen are omitted without renormalization. The displayed second-order correlations use the complete distributions.

Single-mode selection is essential to this factor of two. If $M$ independent equally populated thermal modes are collected together, let $N=\sum_{j=1}^M N_j$ with $\langle N_j\rangle=\mu/M$. Adding their [variances](variance-split.md) gives $\operatorname{Var}N=\mu+\mu^2/M$, hence $g^{(2)}(0)=1+1/M$. Averaging over many unresolved modes can make thermal pair counts approach the independent-count reference.

## ↑ Ancestors (6)

1. [Photon statistics](photon-statistics.md)
2. [Quantum optics](quantum-optics-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Nonclassical state of light](nonclassical-state-of-light.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2013/paper-1/2/b/solution.md)
- [Quantum optics](quantum-optics-split.md)
- [Quantum theory of optical coherence](quantum-theory-of-optical-coherence.md)
- [Siegert relation](siegert-relation.md)
