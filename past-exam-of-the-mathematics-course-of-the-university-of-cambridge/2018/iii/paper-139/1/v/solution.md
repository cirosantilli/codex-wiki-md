<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

First suppose $X$ is integral. Induct on its [dimension of a scheme](../../../../../../dimension-of-a-scheme.md). The previous two parts handle all $j>1$ and also handle $j=1$ when $h^0(X,mD)$ eventually vanishes. Otherwise choose $r>0$ with a nonzero [global section](../../../../../../global-section.md) of $rD$. On an integral variety it defines an [effective Cartier divisor](../../../../../../effective-cartier-divisor.md) $E$, possibly empty, and multiplication by the section gives

$$
0\to\mathcal O_X((m-r)D)\to\mathcal O_X(mD)\to\mathcal O_E(mD)\to0.
$$

Thus $h^1(X,mD)\leq h^1(X,(m-r)D)+h^1(E,mD)$. For $n\geq2$, the induction hypothesis bounds the last term by $O(m^{n-2})$; summing on each residue class modulo $r$ gives $O(m^{n-1})$. For $n=1$, $E$ is zero-dimensional and its positive-degree [sheaf cohomology](../../../../../../sheaf-cohomology.md) vanishes, so the same recurrence is bounded.

For a general [projective scheme](../../../../../../projective-scheme.md), a nonzero section can be a [zero divisor](../../../../../../zero-divisor.md), so that argument requires an additional step. The general [cohomology growth for nef twists](../../../../../../cohomology-growth-for-nef-twists.md) supplies it: for every [coherent sheaf](../../../../../../coherent-sheaf.md) $\mathcal F$ with support dimension $d$,

$$
h^i(X,\mathcal F\otimes\mathcal O_X(mD))=O(m^{d-i})\quad(1\leq i\leq d).
$$

Its proof uses [Fujita vanishing](../../../../../../fujita-vanishing.md), an ample section avoiding the [associated points](../../../../../../associated-point-of-a-coherent-sheaf.md) of $\mathcal F$, and induction on support dimension. Taking $\mathcal F=\mathcal O_X$ gives the required $O(m^{n-1})$ estimate for every $j\geq1$, including nonreduced and reducible schemes; degrees above $n$ vanish.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 139](../../../paper-139-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
