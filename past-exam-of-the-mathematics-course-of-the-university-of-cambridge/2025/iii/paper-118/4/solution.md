<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A Riemannian metric $g$ on a [complex manifold](../../../../../complex-manifold.md) is a Kähler metric when its complex-linear extension is a [Hermitian form](../../../../../hermitian-form.md) on each tangent space and its fundamental two-form

$$
\omega(u,v)=g(Ju,v)
$$

is closed. Equivalently, $\omega$ is a positive real closed $(1,1)$-form, making $X$ a [Kähler manifold](../../../../../kahler-manifold.md).

The [Lefschetz operator of a Kähler manifold](../../../../../lefschetz-operator-of-a-kahler-manifold.md) and its adjoint are

$$
L\alpha=\omega\wedge\alpha,
\qquad \Lambda=L^*.
$$

Because $d\omega=0$ and $\omega$ has type $(1,1)$, both $\partial\omega$ and $\bar\partial\omega$ vanish. The graded [Leibniz rule](../../../../../leibniz-rule.md) therefore gives $[L,\partial]=[L,\bar\partial]=0$.

Writing formal adjoints with stars, define the three [Laplacians](../../../../../laplace-beltrami-operator.md) by

$$
\Delta=dd^*+d^*d,
\qquad
\Delta_\partial=\partial\partial^*+\partial^*\partial,
\qquad
\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial.
$$

The supplied [Kähler identities](../../../../../kahler-identities.md) identity $[\Lambda,\partial]=i\bar\partial^*$ gives, by complex conjugation and taking adjoints,

$$
[\Lambda,\bar\partial]=-i\partial^*,
\qquad [L,\partial^*]=i\bar\partial,
\qquad [L,\bar\partial^*]=-i\partial.
$$

Expanding these commutators and using $\partial\bar\partial+\bar\partial\partial=0$ shows that the mixed terms in $\Delta$ vanish and that $\Delta_\partial=\Delta_{\bar\partial}$. Since $d=\partial+\bar\partial$, it follows that

$$
\Delta=\Delta_\partial+\Delta_{\bar\partial}=2\Delta_\partial=2\Delta_{\bar\partial}.
$$

The adjoint of $[L,\partial]=0$ gives $[\Lambda,\partial^*]=0$. Hence

$$
[\Lambda,\Delta_\partial]=i(\bar\partial^*\partial^*+\partial^*\bar\partial^*)=0,
$$

where the last equality is the adjoint of $\partial\bar\partial+\bar\partial\partial=0$. Thus $\Lambda$, and therefore every power $\Lambda^k$, commutes with $\Delta_\partial$. It follows that $\Lambda^k$ sends every $\partial$-harmonic $(p,q)$-form to a $\partial$-harmonic $(p-k,q-k)$-form whenever $0\leq k\leq\min(p,q)$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 118](../../paper-118-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
