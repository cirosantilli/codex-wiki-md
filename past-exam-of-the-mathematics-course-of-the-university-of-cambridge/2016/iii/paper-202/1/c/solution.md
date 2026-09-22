<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $V$ be the closure of the [simple predictable processes](../../../../../../simple-predictable-process.md) in the [Hilbert space](../../../../../../hilbert-space-split.md) $L^2(\mathcal P,\mu)$. Common refinement of deterministic partitions makes these processes a vector space. To prove **[density of simple predictable processes for finite measures](../../../../../../density-of-simple-predictable-processes-for-finite-measures.md)**, suppose $g\in V^\perp$. Since $\mu$ is a [finite measure](../../../../../../finite-measure.md), the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $g\in L^1(\mu)$, so

$$
\nu(E)=\int_Eg\,d\mu
$$

defines a finite signed [measure](../../../../../../measure.md). The indicator of each predictable generating rectangle, including each time-zero rectangle, is a [simple predictable process](../../../../../../simple-predictable-process.md); hence $\nu$ vanishes on these rectangles.

Finite intersections of the rectangles are again rectangles or empty. Add the whole space to this [pi-system](../../../../../../pi-system.md). Its $\nu$-mass is zero because $\mathbf1_{\Omega\times[0,n]}$ is simple and converges to $1$ in $L^2(\mu)$ by the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md). The zero sets of $\nu$ form a [lambda-system](../../../../../../dynkin-system.md) now that its total mass is zero. The [Pi-lambda theorem](../../../../../../pi-lambda-theorem.md) therefore gives $\nu(E)=0$ for every $E\in\mathcal P$. Taking the sets where $g>0$ and $g<0$ gives $g=0$ $\mu$-almost everywhere.

Thus $V^\perp=\{0\}$ and the [orthogonal complement](../../../../../../orthogonal-complement.md) criterion for a closed subspace of a [Hilbert space](../../../../../../hilbert-space-split.md) yields

$$
\boxed{\overline{\mathcal S}^{\,L^2(\mathcal P,\mu)}=L^2(\mathcal P,\mu).}
$$

Omitting the time-zero term would make this conclusion false when $\mu$ is concentrated at time zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
