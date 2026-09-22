<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [weak derivative](../../../../../weak-derivative.md) condition is

$$
\boxed{\int_\Omega u\,\partial_i\phi\,dx=-\int_\Omega v\phi\,dx\qquad(\phi\in C_c^\infty(\Omega)).}
$$

Both [integrals](../../../../../integral-split.md) exist since $u,v$ are [locally integrable](../../../../../locally-integrable-function.md) and the [test function](../../../../../test-function.md) has [compact support](../../../../../compact-support.md). [Derivatives](../../../../../derivative.md) are defined up to almost-everywhere equality. The space $W^{1,p}(\Omega)$ consists of $u\in L^p(\Omega)$ whose first [weak derivatives](../../../../../weak-derivative.md) $D_i u$ all lie in $L^p(\Omega)$. One standard [norm](../../../../../norm.md) is

$$
\|u\|_{1,p}=\left(\|u\|_p^p+\sum_{i=1}^n\|D_i u\|_p^p\right)^{1/p}\quad(p<\infty),\qquad
\|u\|_{1,\infty}=\max(\|u\|_\infty,\|D_1u\|_\infty,\ldots,\|D_nu\|_\infty).
$$

A sum in the last formula gives an equivalent [norm](../../../../../norm.md). For restriction to $E$, extend any $\phi\in C_c^\infty(E)$ by zero to $\Omega$. Its support is compactly contained in $E$, so the extension is smooth. The identity over $\Omega$ then reduces exactly to the identity over $E$, proving locality of the [weak derivative](../../../../../weak-derivative.md).

For the [jump contribution to a piecewise weak derivative](../../../../../jump-contribution-to-a-piecewise-weak-derivative.md), [integration by parts](../../../../../integration-by-parts.md) on the two sides of the joining point gives the [distributional derivative](../../../../../distributional-derivative.md)

$$
Du=2x\,\mathbf1_{(0,1)}+\mathbf1_{(1,2)}+(a-1)\delta_1.
$$

The coefficient is the right [trace](../../../../../trace-operator.md) $1+a$ minus the left [trace](../../../../../trace-operator.md) $2$. If a [locally integrable](../../../../../locally-integrable-function.md) [weak derivative](../../../../../weak-derivative.md) existed, locality on each open side would identify it [almost everywhere](../../../../../almost-everywhere.md) with the displayed regular part. Substituting that into the global test identity would force $(a-1)\phi(1)=0$ for every [test function](../../../../../test-function.md), hence $a=1$. Equivalently a nonzero Dirac [point mass](../../../../../dirac-delta-function.md) cannot be represented by a [locally integrable](../../../../../locally-integrable-function.md) [derivative](../../../../../derivative.md).

For $a=1$ the [point-mass](../../../../../dirac-delta-function.md) term vanishes, and both the [function](../../../../../function-split.md) and its piecewise [derivative](../../../../../derivative.md) are [bounded](../../../../../boundedness.md) on the finite [interval](../../../../../interval-mathematics.md). Thus $u\in W^{1,\infty}$ and hence in every listed $W^{1,p}$. Therefore **membership holds exactly for $a=1$**. Changing a single point value is irrelevant to Sobolev membership; it cannot remove mismatched [one-sided traces](../../../../../trace-operator.md) when $a\ne1$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../split.md)
6. [Methods of applied functional analysis course of the University of Oxford](../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
