<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [free algebra functor](../../../../../../free-algebra-functor.md) is

$$
F(A)=(TA,\mu_A),\qquad F(f)=Tf.
$$

The [monad](../../../../../../monad.md) laws make $\mu_A$ an algebra action, and naturality of $\mu$ makes $Tf$ a [morphism of algebras for a monad](../../../../../../morphism-of-algebras-for-a-monad.md). Let $U:\mathcal C^T\to\mathcal C$ forget the action. Define

$$
\boxed{\mathcal C^T(F A,(B,b))\cong\mathcal C(A,B),\qquad
h\longmapsto h\eta_A,\quad f\longmapsto bTf.}
$$

The proposed inverse is an algebra morphism because

$$
(bTf)\mu_A=b\mu_B T^2f=bTb\,T^2f=bT(bTf).
$$

Naturality of $\eta$ and the algebra unit law give $(bTf)\eta_A=f$. If $h$ is an algebra morphism, then

$$
bT(h\eta_A)=bTh\,T\eta_A=h\mu_A T\eta_A=h.
$$

The formulas are natural in both variables, so **$F\dashv U$**. Its unit is $\eta$, and its counit at $(B,b)$ has underlying map $b:TB\to B$. Thus the [monad induced by an adjunction](../../../../../../monad-induced-by-an-adjunction.md) has endofunctor $UF=T$, unit $\eta$, and multiplication $U\varepsilon_F=\mu$. It is **exactly the original monad**, not merely a monad with the same endofunctor.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
