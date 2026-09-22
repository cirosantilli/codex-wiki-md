<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix the reference bit-flip chain

$$
E_{s,q}=E_s\bar X^q
$$

and assign to each lattice edge $e=vv'$ the bond sign

$$
\eta_{vv'}(s,q)=(-1)^{n_e(E_{s,q})},
$$

where $n_e(E)=1$ if $E$ contains $X_e$ and is zero otherwise. A product of star stabilizers is specified by Ising spins $\sigma_v$: choose the star at $v$ when $\sigma_v=-1$. The resulting error has edge occupation

$$
n_e=\frac{1-\eta_{vv'}\sigma_v\sigma_{v'}}2.
$$

For $N$ edges, its independent bit-flip probability is

$$
p^{|E|}(1-p)^{N-|E|}
=[p(1-p)]^{N/2}
\exp\left(\beta J\sum_{vv'}
\eta_{vv'}\sigma_v\sigma_{v'}\right),
$$

because $e^{\beta J}=\sqrt{(1-p)/p}$. Summing over products of stars therefore gives the [Surface-code decoding as a random-bond Ising model](../../../../../../surface-code-decoding-as-a-random-bond-ising-model.md) identity

$$
\Pr(E\in E_s\bar X^qS_X)
=\frac{[p(1-p)]^{N/2}}{r}\,Z_{s,q},
$$

where $r$ is the number of Ising configurations representing the same stabilizer product, usually $r=2$ on a closed connected lattice because a global spin flip changes no bond. The class-independent prefactor cancels when the two logical classes $q=0,1$ are compared.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
