<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix a [coherent sheaf](../../../../coherent-sheaf.md) $F$ and an integer $k>M$. Set $K_0=F$. Repeatedly apply [a](../a.md) to construct [short exact sequences of sheaves](../../../../short-exact-sequence-of-sheaves.md)

$$
0\longrightarrow K_{j+1}\longrightarrow G_j\longrightarrow K_j\longrightarrow0,
$$

where each $G_j$ is a [coherent sheaf](../../../../coherent-sheaf.md) and a [locally free sheaf](../../../../locally-free-sheaf.md). Each [kernel sheaf](../../../../kernel-sheaf.md) $K_{j+1}$ is a [coherent sheaf](../../../../coherent-sheaf.md) because $X$ is a [noetherian scheme](../../../../noetherian-scheme.md). Thus the construction can be repeated as many times as needed; it does not require the [kernel sheaves](../../../../kernel-sheaf.md) themselves to be [locally free sheaves](../../../../locally-free-sheaf.md).

For every integer $q>M$, the [long exact sequence in sheaf cohomology](../../../../long-exact-sequence-in-sheaf-cohomology.md) contains

$$
H^q(X,G_j)\longrightarrow H^q(X,K_j)\xrightarrow{\ \delta_j\ }H^{q+1}(X,K_{j+1})\longrightarrow H^{q+1}(X,G_j).
$$

Both outer groups vanish by the hypothesis, since $q$ and $q+1$ exceed $M$. Hence $\delta_j$ is an [isomorphism](../../../../isomorphism.md). Iterating this [dimension shifting in sheaf cohomology](../../../../dimension-shifting-in-sheaf-cohomology.md) gives

$$
H^k(X,F)\cong H^{k+1}(X,K_1)\cong\cdots\cong H^{k+s}(X,K_s).
$$

Choose $s\geq0$ with $k+s>N$, where $N$ is the uniform bound from [b](../b.md). The [coherent sheaf](../../../../coherent-sheaf.md) $K_s$ is a [quasi-coherent sheaf](../../../../quasi-coherent-sheaf.md), so [b](../b.md) makes the last group zero. Therefore

$$
\boxed{H^k(X,F)=0\quad\text{for every coherent sheaf }F\text{ and every }k>M.}
$$

The argument uses a finite initial segment of a [locally free resolution](../../../../locally-free-resolution.md). There is no need to assume that every [coherent sheaf](../../../../coherent-sheaf.md) has a finite [locally free resolution](../../../../locally-free-resolution.md): the uniform bound from [b](../b.md) is what terminates the argument.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
