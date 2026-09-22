<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Expand in the [Fourier sine basis](../../../../../fourier-sine-basis.md), using unnormalized [eigenfunctions](../../../../../eigenfunction.md):

$$
f(x)=\sum_{n=1}^\infty f_n\sin\frac{n\pi x}{l},\qquad
f_n=\frac2l\int_0^lf(t)\sin\frac{n\pi t}{l}\,dt,
\qquad y(x)=\sum_{n=1}^\infty c_n\sin\frac{n\pi x}{l}.
$$

Projection of $\mathcal Ly=f$ onto each [eigenfunction](../../../../../eigenfunction.md) gives

$$
\boxed{\left[1-\left(\frac{n\pi}{l}\right)^2\right]c_n=f_n.}
$$

When $l\notin\pi\mathbb N_{>0}$, every [eigenvalue](../../../../../eigenvalue.md) is nonzero and the [eigenfunction expansion](../../../../../eigenfunction-expansion.md) is uniquely determined:

$$
\boxed{y(x)=\sum_{n=1}^\infty
\frac{f_n}{1-(n\pi/l)^2}\sin\frac{n\pi x}{l}.}
$$

When $l=m\pi$, the exceptional index is $n=m$, for which the [eigenfunction](../../../../../eigenfunction.md) is $\sin x$. If $f_m\ne0$, its coefficient equation is $0=f_m$, an inconsistency: there is no solution. If $f_m=0$, the coefficient equation is $0=0$, and $c_m$ is arbitrary. The full family is

$$
\boxed{y(x)=C\sin x+
\sum_{\substack{n\geq1\\n\ne m}}
\frac{f_n}{1-(n/m)^2}\sin\frac{nx}{m},\qquad C\in\mathbb R.}
$$

This is the [Fredholm alternative](../../../../../fredholm-alternative.md) directly in the coefficient equations: nonzero [eigenvalues](../../../../../eigenvalue.md) fix their coefficients; a zero [eigenvalue](../../../../../eigenvalue.md) requires zero forcing in that direction and leaves the corresponding coefficient free. An inconsistent equation at a zero [eigenvalue](../../../../../eigenvalue.md) cannot be repaired by assigning an infinite coefficient.

For convergence, [Lipschitz continuity](../../../../../lipschitz-continuity.md) implies [absolute continuity](../../../../../absolutely-continuous-function.md) of $f$, with bounded [derivative](../../../../../derivative.md) almost everywhere. One [integration by parts](../../../../../integration-by-parts.md) gives $f_n=O(n^{-1})$; since the denominators grow quadratically, $c_n=O(n^{-3})$ apart from the single free coefficient. The solution series and its first [derivative](../../../../../derivative.md) therefore converge uniformly. The second [derivative](../../../../../derivative.md) converges in $L^2$, and the resulting [Sobolev space](../../../../../sobolev-space-split.md) solution satisfies $y''=f-y$. As $f-y$ is a [continuous function](../../../../../continuous-function.md), this is a classical $C^2$ solution, with both [boundary conditions](../../../../../boundary-condition.md) satisfied. The forcing's [Fourier sine series](../../../../../fourier-sine-series.md) is interpreted on the open interval or in $L^2$; its endpoint values need not equal the endpoint values of $f$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
