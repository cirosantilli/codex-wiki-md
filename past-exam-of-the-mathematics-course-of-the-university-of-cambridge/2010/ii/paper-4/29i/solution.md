<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

Write $s=S_0$, assume the usual nonzero initial price vector, and define

$$
A=s^TV^{-1}s,\quad B=s^TV^{-1}\mu,\quad C=\mu^TV^{-1}\mu,\quad
D=AC-B^2.
$$

The [covariance matrix](../../../../../covariance-matrix.md) $V$ is positive definite. If $s,\mu$ are linearly independent, then $D>0$ by the strict [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). The [Lagrangian](../../../../../lagrangian.md) for [mean-variance optimization](../../../../../modern-portfolio-theory.md) can be written

$$
\mathcal L(\pi,\lambda,\eta)=\frac12\pi^TV\pi
-\lambda(s^T\pi-x)-\eta(\mu^T\pi-m).
$$

Its first-order equation gives $\pi=\lambda V^{-1}s+\eta V^{-1}\mu$. The two constraints then give

$$
\boxed{\pi=\frac{Cx-Bm}{D}\pi_A+\frac{Am-Bx}{D}\pi_B,\qquad
\pi_A=V^{-1}s,\quad\pi_B=V^{-1}\mu.}
$$

Strict convexity makes this the unique constrained minimizer. Its [variance](../../../../../variance-split.md) is

$$
\boxed{v_{\min}(m)=\frac{Cx^2-2Bxm+Am^2}{D}
=\frac{x^2}{A}+\frac A D\left(m-\frac{Bx}{A}\right)^2.}
$$

The [mean-variance efficient frontier](../../../../../efficient-frontier.md) is the upper branch $m\ge Bx/A$: points on the lower branch have a larger-mean competitor of the same [variance](../../../../../variance-split.md). The picture shows the generic nondegenerate case at a fixed initial budget. With only two stocks and independent budget and mean constraints, every feasible portfolio lies on the curve; additional independent portfolio directions allow larger variances at the same mean.<a id="29i/image-mean-variance-frontier-with-its-efficient-upper-branch-and-minimum-variance-portfolio"></a>


![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4-frontier.png)

**[Figure 1](#29i/image-mean-variance-frontier-with-its-efficient-upper-branch-and-minimum-variance-portfolio). Mean–variance frontier with its efficient upper branch and minimum-variance portfolio**.

If $\mu=\kappa s$, then $D=0$, and only $m=\kappa x$ is feasible. The [variance](../../../../../variance-split.md) minimizer is $(x/A)V^{-1}s$, still in the stated span; no two-dimensional frontier exists. This degeneracy is not excluded merely by nonsingularity of $V$.

For exponential utility and Gaussian prices, the [moment-generating function](../../../../../moment-generating-function.md) gives

$$
\mathbb EU(\pi^TS_1)
=-\exp\left(-\gamma\mu^T\pi+\frac{\gamma^2}2\pi^TV\pi\right).
$$

Maximizing this is equivalent to maximizing $\mu^T\pi-\gamma\pi^TV\pi/2$ subject to $s^T\pi=y$. Its strictly concave first-order equation gives

$$
\boxed{\pi=\frac1\gamma V^{-1}\mu-\frac\eta\gamma V^{-1}s,\qquad
\eta=\frac{B-\gamma y}{A}.}
$$

Thus the same two funds suffice.

For the [Gaussian two-fund theorem](../../../../../gaussian-two-fund-theorem.md) with general utility, the Gaussian assumption and the exponential growth bounds justify the differentiations and expectations. Gaussian integration by parts applied to $S_1=\mu+V^{1/2}Z$ gives

$$
\mathbb E[S_1U'(\pi^TS_1)]
=\mu\,\mathbb EU'(\pi^TS_1)+V\pi\,\mathbb EU''(\pi^TS_1).
$$

At any finite maximizer the left side is a multiplier $\eta s$. If $U$ is concave and non-affine, and $\pi\ne0$, then $\pi^TS_1$ is a nondegenerate Gaussian with positive density everywhere. Since continuous $U''\le0$ is strictly negative on some interval, its expectation is strictly negative. Rearranging proves

$$
\boxed{\pi=
\frac{\eta V^{-1}s-\mathbb EU'(\pi^TS_1)V^{-1}\mu}
{\mathbb EU''(\pi^TS_1)}
\in\operatorname{span}\{\pi_A,\pi_B\}.}
$$

The zero portfolio already belongs to that span.

There is a genuine qualification in the final printed assertion: increasing and concave does not exclude affine utility. For $U(w)=w$, $s=\mu=(1,1,1)^T$, and $V=I$, every budget-feasible portfolio is optimal. With $y=1$, $(1,0,0)^T$ is optimal but is outside the common line spanned by $\pi_A,\pi_B$. If $\mu$ is not proportional to $s$, affine utility has no maximizer at all, because a zero-cost direction with positive mean can be scaled without bound. Thus the universal claim about the maximizing portfolio needs non-affine utility and existence of a finite maximizer. Under the literal weaker assumptions there is still a two-fund optimum whenever an optimum exists: the affine constant-mean case permits choosing the minimum-variance portfolio.

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
