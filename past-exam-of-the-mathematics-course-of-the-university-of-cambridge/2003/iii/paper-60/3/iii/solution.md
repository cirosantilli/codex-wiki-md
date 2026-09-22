<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

At a periodic steady state, two spatial integrations of $0=(B+\delta A^2)_{XX}$ make $B+\delta A^2$ constant. The zero-mean constraint fixes that constant to $\delta\langle A^2\rangle$. Define $\beta=1-\delta>0$ and $\nu=\mu-\delta\langle A^2\rangle$; the stationary [amplitude equation](../../../../../../amplitude-equation.md) is

$$
A_{XX}+\nu A+\alpha A^2-\beta A^3=0,\qquad B=\delta(\langle A^2\rangle-A^2).
$$

For a broad localized plateau, the two transition layers occupy $O(\ell)$ length while the plateau and exterior occupy $2hL$ and $2(1-h)L$. Provided both lengths are large compared with the [front](../../../../../../front-solution.md) width $\ell$, spatial averaging gives $\langle A^2\rangle=hR^2+O(R^2\ell/L)$.

Multiplying the stationary equation by $A_X$ gives the [first integral](../../../../../../first-integral.md)

$$
\frac12A_X^2+W(A)=E,\qquad W(A)=\frac\nu2A^2+\frac\alpha3A^3-\frac\beta4A^4.
$$

In the well-separated-front approximation, $A\to0$ with $A_X\to0$ outside, so $E=0$. On the plateau $A\to R\ne0$, giving both $\nu+\alpha R-\beta R^2=0$ and $W(R)=0$. Substitution of the first into the second gives $R^3(\beta R/4-\alpha/6)=0$, hence

$$
\boxed{R=\frac{2\alpha}{3\beta},\qquad \nu=-\frac{2\alpha^2}{9\beta}.}
$$

The equal-potential condition is therefore $2\alpha^2=-9\nu\beta$. It is a [front](../../../../../../front-solution.md) balance, not an integration of the stationary equation without its $A_X$ multiplier.

These plateau values also produce actual isolated [fronts](../../../../../../front-solution.md). At this balance $W(A)=-\beta A^2(A-R)^2/4$, so for $\alpha>0$ the increasing [front](../../../../../../front-solution.md) satisfies $A_X=\sqrt{\beta/2}\,A(R-A)$. It is

$$
A(X)=\frac{R}{1+\exp[-R\sqrt{\beta/2}(X-X_0)]},\qquad \ell=\frac1{R\sqrt{\beta/2}}.
$$

For $\alpha<0$ the sign-reversed construction gives the negative plateau. Two oppositely oriented well-separated [fronts](../../../../../../front-solution.md) give the leading periodic [mesa solution](../../../../../../mesa-solution.md) approximation; their weak interaction and tails supply finite-$L$ corrections.

Finally $\nu=\mu-\delta hR^2$ gives the [coexistence fraction of a conserved-field amplitude mesa](../../../../../../coexistence-fraction-of-a-conserved-field-amplitude-mesa.md):

$$
\boxed{h(\mu)=\frac{9(1-\delta)^2\mu}{4\delta\alpha^2}+\frac{1-\delta}{2\delta}.}
$$

The leading existence range is the interval obtained from $0<h<1$:

$$
\boxed{-\frac{2\alpha^2}{9(1-\delta)}<\mu<\frac{2\alpha^2(3\delta-1)}{9(1-\delta)^2},\qquad 0<\delta<1.}
$$

This assumes $\alpha\ne0$ and $L\gg\ell$, with $hL,(1-h)L\gg\ell$. At the two displayed ends a transition pair can no longer be treated as well separated, so they are asymptotic bounds rather than exact finite-period [bifurcation](../../../../../../bifurcation.md) values. For $\alpha=0$ this particular nonzero plateau balance collapses to $R=0$ and does not yield the [mesa solution](../../../../../../mesa-solution.md) family.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
