<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $m=\dim M$ and $n=\dim N$. The hypothesis says that $q$ is a [regular value](../../../../../../regular-value.md) of $F$. Since its preimage is nonempty and the [differential of a smooth map](../../../../../../differential-of-a-smooth-map.md) is surjective there, $m\geq n$.

We use the following finite-dimensional [inverse function theorem](../../../../../../inverse-function-theorem.md): if a smooth map $H:O\to\mathbb R^m$, with $O\subset\mathbb R^m$ open, has invertible derivative at $a$, there are open neighborhoods of $a$ and $H(a)$ on which $H$ is a [diffeomorphism](../../../../../../diffeomorphism.md), with smooth inverse.

Fix $p\in F^{-1}(q)$. Choose [coordinate charts](../../../../../../manifold-chart.md) centered at $p$ and $q$, and shrink the source neighborhood so that its image under $F$ lies in the target chart. Its coordinate expression is $f=(f^1,\ldots,f^n)$ with $f(0)=0$ and derivative of rank $n$. Choose $n$ domain coordinates giving an invertible $n\times n$ minor, and relabel them as $x^1,\ldots,x^n$. Define

$$
H(x)=\bigl(f^1(x),\ldots,f^n(x),x^{n+1},\ldots,x^m\bigr).
$$

Its derivative at zero has block form

$$
DH_0=\begin{pmatrix}B&C\\0&I_{m-n}\end{pmatrix},\qquad \det B\ne0,
$$

so it is invertible. The [inverse function theorem](../../../../../../inverse-function-theorem.md) makes $u=H(x)$ a new [coordinate chart](../../../../../../manifold-chart.md) near $p$. In this chart $F=q$ is exactly $u^1=\cdots=u^n=0$, because the target chart sends $q$ to zero. These are [slice charts for an embedded submanifold](../../../../../../slice-chart-for-an-embedded-submanifold.md); reordering coordinates if desired puts the free coordinates first. Giving the level set the [subspace topology](../../../../../../subspace-topology.md), these restricted charts are smoothly compatible, as in part (a). This proves the [regular level set theorem](../../../../../../regular-level-set-theorem.md) rather than merely invoking it.

**The level set is an embedded submanifold of dimension $\boxed{m-n}$**. The same coordinates show $T_pZ=\ker dF_p$: tangent vectors to the slice have zero first $n$ components, which are exactly the components of $dF_p$. The empty-dimensional case $m=n$ gives a discrete zero-dimensional [embedded submanifold](../../../../../../embedded-submanifold.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
