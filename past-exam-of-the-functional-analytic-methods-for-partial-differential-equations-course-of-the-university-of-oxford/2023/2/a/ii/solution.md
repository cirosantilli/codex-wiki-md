<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\psi\in C_c^\infty(B_1)$, the functions $\psi$ and $\partial_i\psi$ are bounded. Hence $\psi u$ and $\psi\partial_i u+u\partial_i\psi$ belong to $L^p(B_1)$. For a [test function](../../../../../test-function.md) $\phi$, the classical [product rule](../../../../../product-rule.md) and the [weak derivative](../../../../../weak-derivative.md) identity for $u$, tested with $\psi\phi$, give

$$
\begin{aligned}
\int_{B_1}\psi u\,\partial_i\phi
&=\int_{B_1}u\,\partial_i(\psi\phi)-\int_{B_1}u(\partial_i\psi)\phi\\
&=-\int_{B_1}\bigl(\psi\partial_i u+u\partial_i\psi\bigr)\phi.
\end{aligned}
$$

Therefore

$$
\boxed{\psi u\in W^{1,p}(B_1),\qquad
\partial_i(\psi u)=\psi\partial_i u+u\partial_i\psi.}
$$

In fact $\psi u$ has [compact support](../../../../../compact-support.md) in $B_1$ and belongs to the corresponding zero-boundary [Sobolev space](../../../../../sobolev-space-split.md), by [mollification](../../../../../mollification.md) within that support.

For arbitrary $\psi\in C^\infty(B_1)$, the same identity still proves the local [product rule](../../../../../product-rule.md) for [weak derivatives](../../../../../weak-derivative.md), but membership in the global [Sobolev space](../../../../../sobolev-space-split.md) can fail. To give a counterexample for every dimension and every $p$ in the question, take

$$
u\equiv1,\qquad\psi(x)=\frac1{1-|x|^2}.
$$

Here $u\in W^{1,p}(B_1)$ and $\psi$ is a [smooth function](../../../../../smooth-function.md) on the open ball, while [polar coordinates](../../../../../polar-coordinates.md) show

$$
\int_{B_1}|\psi|^p\,dx
\geq c_n\int_{1/2}^1(1-r^2)^{-p}\,dr=\infty\qquad(p\geq1).
$$

Thus $\psi u\notin L^p(B_1)$, and the global assertion is false. Boundedness of $\psi$ and its first [derivatives](../../../../../derivative.md) would suffice without [compact support](../../../../../compact-support.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
