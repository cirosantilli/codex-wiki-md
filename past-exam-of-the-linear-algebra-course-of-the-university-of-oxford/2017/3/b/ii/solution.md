<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Differentiate the expression from the source before applying any finite-dimensional result. The exponential factors cancel:

$$
\boxed{Tf=f''-2xf'-2f.}
$$

This is a [polynomial](../../../../../polynomial-split.md) whenever $f$ is a [polynomial](../../../../../polynomial-split.md), and its [polynomial degree](../../../../../degree-of-a-polynomial.md) is at most that of $f$. Differentiation and multiplication are linear, so $T$ is a [linear transformation](../../../../../linear-map.md) $V\to V$, and every $V_n$ is an [invariant subspace](../../../../../invariant-subspace.md).

For [self-adjointness](../../../../../self-adjoint-operator.md), put $w(x)=e^{-x^2}$. Then $w'=-2xw$ and $wTf=(wf')'-2wf$. [Integration by parts](../../../../../integration-by-parts.md) therefore gives

$$
\begin{aligned}
\langle Tf,g\rangle
&=\int_{-\infty}^{\infty}\bigl((w\overline{f'})'-2w\overline f\bigr)g\,dx\\
&=-\int_{-\infty}^{\infty}w\overline{f'}g'\,dx
-2\int_{-\infty}^{\infty}w\overline f g\,dx\\
&=\langle f,Tg\rangle.
\end{aligned}
$$

The discarded endpoint terms are $w\overline{f'}g$ and $w\overline f g'$. They vanish at both infinities because exponential decay dominates every [polynomial](../../../../../polynomial-split.md). The same decay justifies the intermediate integrals. Consequently

$$
\boxed{T(V_n)\subseteq V_n,\qquad
\langle Tf,g\rangle=\langle f,Tg\rangle\quad(f,g\in V).}
$$

Here the question's [self-adjointness](../../../../../self-adjoint-operator.md) is in the sense of an [adjoint on an inner product space](../../../../../adjoint-on-an-inner-product-space.md): $T$ itself represents the adjoint on the polynomial space. Each finite-dimensional restriction $T|_{V_n}$ is a [self-adjoint operator](../../../../../self-adjoint-operator.md). No choice of operator domain in a completed [Hilbert space](../../../../../hilbert-space-split.md) is needed for this argument. The resulting [Gaussian polynomial operator](../../../../../gaussian-polynomial-operator.md) will produce [Hermite polynomials](../../../../../hermite-polynomial.md) in part (iv).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
