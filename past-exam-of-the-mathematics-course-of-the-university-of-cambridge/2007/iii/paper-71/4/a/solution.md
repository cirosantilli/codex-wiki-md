<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Fourier sine basis](../../../../../../fourier-sine-basis.md) of the unit square is $e_{j\ell}(x,y)=2\sin(j\pi x)\sin(\ell\pi y)$, $j,\ell\geq1$, normalized in the [L2 inner product](../../../../../../l2-inner-product.md). It satisfies the zero [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) and $\Delta e_{j\ell}=-\pi^2(j^2+\ell^2)e_{j\ell}$. Expand the given initial datum as $u_0=\sum a_{j\ell}e_{j\ell}$, where $\sum|a_{j\ell}|^2=\|u_0\|_2^2$. The solution is

$$
u(x,y,t)=\sum_{j,\ell\geq1}a_{j\ell}e^{[\kappa-\pi^2(j^2+\ell^2)]t}e_{j\ell}(x,y).
$$

For $\kappa\leq2\pi^2$, every exponent is nonpositive. The series converges in $L^2$ for $t\geq0$, tends to $u_0$ in $L^2$ as $t\downarrow0$ by dominated convergence, and differentiates termwise for $t>0$ because the Gaussian high-frequency decay dominates every polynomial derivative factor. This constructs a classical positive-time solution and the appropriate mild solution at the possibly rough initial time.

Its norm and the difference of two such solutions satisfy

$$
\boxed{\|u(t)\|_2\leq e^{(\kappa-2\pi^2)t}\|u_0\|_2,\qquad\|u(t)-v(t)\|_2\leq e^{(\kappa-2\pi^2)t}\|u_0-v_0\|_2.}
$$

Existence, uniqueness in the natural $L^2$ solution class, and continuous dependence follow. For uniqueness one can project any weak solution onto each sine mode, obtaining the same scalar linear equation and initial coefficient. Thus this is a [Hadamard well-posed problem](../../../../../../well-posed-problem.md), with a contractive [strongly continuous semigroup](../../../../../../c0-semigroup.md) in the stated range.

To prove pointwise decay from merely $L^2$ data, use $|e_{j\ell}|\leq2$ and the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md):

$$
\sup_{x,y}|u(x,y,t)|\leq2\|u_0\|_2\left(\sum_{j,\ell\geq1}e^{2[\kappa-\pi^2(j^2+\ell^2)]t}\right)^{1/2}.
$$

For $t\geq1$, factor out $e^{2(\kappa-2\pi^2)t}$; the remaining sum is bounded by $\sum_{j,\ell\geq1}e^{-2\pi^2(j^2+\ell^2-2)}<\infty$. Therefore

$$
\boxed{\kappa<2\pi^2\quad\Longrightarrow\quad\sup_{(x,y)\in[0,1]^2}|u(x,y,t)|\longrightarrow0.}
$$

At equality the first sine mode is stationary, so strict inequality is essential for decay of every datum. This is the [Dirichlet heat-reaction threshold on the unit square](../../../../../../dirichlet-heat-reaction-threshold-on-the-unit-square.md). The equation is actually well posed on every fixed finite time interval for any fixed real $\kappa$; beyond the threshold it has a growing first mode and loses long-time contractivity. The restricted well-posedness assertion in the question is therefore sufficient rather than necessary.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
