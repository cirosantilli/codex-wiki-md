<h1 id="21i/solution">Solution</h1>

↑ **Parent:** [21I](../21i.md)

Chain maps $f,g:C_*\to C_*'$ are [chain homotopic](../../../../../chain-homotopy.md) when maps $h_n:C_n\to C'_{n+1}$ satisfy

$$
f-g=\partial h+h\partial.
$$

For a cycle $z$, $f(z)-g(z)=\partial h(z)$ is a boundary, so $f_*=g_*$ on homology.

Fix a vertex $e_0$ of $\Delta^n$ and define the cone operator by adjoining $e_0$ to an oriented simplex, with zero when it is already present. The simplicial boundary formula gives

$$
\partial h+h\partial=\operatorname{id}
$$

on the reduced chain complex. Thus its identity is null-homotopic and

$$
\widetilde H_k(\Delta^n)=0
$$

for every $k$; equivalently, $H_0(\Delta^n)\cong\mathbb Z$ and higher homology vanishes.

For the 2-skeleton $K$ of $\Delta^6$,

$$
\dim C_0=7,
\quad\dim C_1=21,
\quad\dim C_2=35.
$$

It is connected and simply connected, so $H_0\cong\mathbb Z$ and $H_1=0$. Euler characteristic then gives

$$
21=1+\operatorname{rank}H_2,
\qquad
\boxed{H_2(K)\cong\mathbb Z^{20}}.
$$

For $\sigma=(0123)(456)$, no vertex or edge is fixed. The only invariant 2-simplex is $[456]$, on which the 3-cycle preserves orientation, so the chain traces are $0,0,1$. The [Lefschetz trace formula](../../../../../lefschetz-number.md) gives

$$
1=\operatorname{tr}(f_*|H_0)+\operatorname{tr}(f_*|H_2),
$$

therefore

$$
\boxed{\operatorname{tr}(f_*|H_2(K;\mathbb Q))=0}.
$$

## ↑ Ancestors (10)

1. [21I](../21i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
