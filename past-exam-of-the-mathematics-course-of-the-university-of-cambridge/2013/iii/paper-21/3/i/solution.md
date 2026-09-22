<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a finite [Galois extension](../../../../../../finite-galois-extension.md) of local fields, let $G=\operatorname{Gal}(L/K)$, $G_{-1}=G$, and, for integers $i\geq0$, define the lower [ramification groups](../../../../../../ramification-group.md) by

$$
G_i=\{\sigma\in G:v_L(\sigma(a)-a)\geq i+1\text{ for all }a\in\mathcal O_L\}.
$$

In particular, $G_0$ is the [inertia group](../../../../../../inertia-group.md). The identity satisfies every bound because $v_L(0)=\infty$.

If the extension is [totally ramified](../../../../../../totally-ramified-extension.md), its [residue fields](../../../../../../residue-field.md) agree. Choose representatives in $\mathcal O_K$ of their common [residue field](../../../../../../residue-field.md). Every $a\in\mathcal O_L$ has a convergent [uniformiser](../../../../../../uniformizer.md) expansion $a=\sum_{j\geq0}c_j\pi_L^j$ with these representatives $c_j$, all fixed by $G$. For $j\geq1$,

$$
\sigma(\pi_L)^j-\pi_L^j=(\sigma(\pi_L)-\pi_L)\sum_{r=0}^{j-1}\sigma(\pi_L)^r\pi_L^{j-1-r}.
$$

Each summand in the second factor has [valuation](../../../../../../valuation.md) $j-1$. Thus a bound $v_L(\sigma(\pi_L)-\pi_L)\geq i+1$ implies the same bound on $\sigma(a)-a$, by convergence and the [valuation](../../../../../../valuation.md) inequality. Necessity follows by testing $a=\pi_L$. This proves the [uniformizer criterion for lower ramification groups](../../../../../../uniformizer-criterion-for-lower-ramification-groups.md):

$$
\boxed{G_i=\{\sigma\in G:v_L(\sigma(\pi_L)-\pi_L)\geq i+1\}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
