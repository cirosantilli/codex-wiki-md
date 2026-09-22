<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [de Rham cohomology](../../../../../../de-rham-cohomology.md) is

$$
H^p_{\mathrm{dR}}(M)=\ker(d:\Omega^p\to\Omega^{p+1})/operatorname{im}(d:\Omega^{p-1}\to\Omega^p).
$$

The [Poincaré lemma](../../../../../../poincare-lemma.md) says that every closed positive-degree differential form is locally exact, and is exact on every star-shaped open subset of Euclidean space.

Let $n>1$ and let $\alpha$ be a closed one-form on $M$. The hypothesis gives $\alpha=dg$ on $M\setminus B$. Choose a slightly larger coordinate ball $B'$ around $B$. The Poincare lemma gives $\alpha=dh$ on $B'$. The annulus $B'\setminus B$ is connected when $n>1$, so $d(g-h)=0$ there and $g-h$ is constant. Adjusting $h$ by this constant makes $g$ and $h$ agree on the overlap, and they glue to a global primitive of $\alpha$. Hence $H^1(M)=0$. For $n=1$ the claim fails: remove a closed proper interval from $S^1$. Its complement is an interval and has vanishing first de Rham cohomology, whereas $H^1(S^1)\cong\mathbb R$.

Finally choose a nowhere-vanishing $n$-form $\omega$ on $S^n$ and a coordinate $t$ on the finite interval $I$. Every $(n+1)$-form on $S^n\times I$ is $a(x,t)\omega\wedge dt$. Fix $t_0\in I$ and put

$$
A(x,t)=\int_{t_0}^t a(x,s)\,ds.
$$

Since $d_{S^n}A\wedge\omega=0$ for dimensional reasons,

$$
d((-1)^nA\omega)=a\omega\wedge dt.
$$

Every top-degree form is exact, so $H^{n+1}(S^n\times I)=0$ without using the de Rham theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
