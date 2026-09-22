<h1 id="14e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

After division by $z$, the coefficient functions are

$$
P(z)=\frac1z-1,
\qquad Q(z)=\frac\lambda z.
$$

Both $zP(z)=1-z$ and $z^2Q(z)=\lambda z$ are analytic at zero, so the [regular singular point criterion for a second-order equation](../../../../../../regular-singular-point-criterion-for-a-second-order-equation.md) shows that $z=0$ is regular singular. Substitution of $y=z^r$ into the leading terms gives the indicial equation

$$
r(r-1)+r=r^2=0.
$$

The exponent is repeated. Directly substituting $y=\sum_{n\geq0}a_nz^n$ gives

$$
(n+1)^2a_{n+1}+(\lambda-n)a_n=0,
\qquad
\boxed{a_{n+1}=\frac{n-\lambda}{(n+1)^2}a_n}.
$$

Thus $a_0$ determines the entire power series, so there is only one such solution $y_1$ up to scale. The [logarithmic solution from a repeated Frobenius exponent](../../../../../../logarithmic-solution-from-a-repeated-frobenius-exponent.md) predicts

$$
\boxed{y_2(z)=y_1(z)\log z+\text{a power series}},
$$

so its leading nonanalytic term is proportional to $\log z$.

For the contour ansatz, differentiation under the integral and one integration by parts give

$$
\begin{aligned}
0={}&\int_\gamma e^{zt}
 \{z(t^2-t)+(t+\lambda)\}f(t)\,dt\\
={}&\left[e^{zt}t(t-1)f(t)\right]_{\partial\gamma}
 +\int_\gamma e^{zt}
 \left\{(t+\lambda)f-[t(t-1)f]'\right\}dt.
\end{aligned}
$$

The integral vanishes when

$$
t(t-1)f'+(t-1-\lambda)f=0,
$$

whose solution is the [Laguerre contour-integral amplitude](../../../../../../laguerre-contour-integral-amplitude.md)

$$
\boxed{f(t)=t^{-\lambda-1}(t-1)^\lambda}.
$$

The contour and branches must make $f$ single-valued along the traversed path and must kill the endpoint term

$$
\left[e^{zt}t^{-\lambda}(t-1)^{\lambda+1}\right]_{\partial\gamma}.
$$

Now suppose $\lambda<0$ is nonintegral. Near $t=0$, $f(t)=O(t^{-\lambda-1})$ is integrable and the endpoint factor is $O(t^{-\lambda})\to0$. We may therefore choose

$$
\gamma_1:quad 0\longrightarrow
\text{one counterclockwise loop around }1
\longrightarrow0,
$$

a finite loop based at the branch point $0$ and avoiding $1$ except by encirclement. A second choice is

$$
\gamma_2:quad 0\longrightarrow-\infty
$$

along one bank of the negative real axis, with a consistent branch. At $-\infty$, $e^{zt}$ kills the algebraic endpoint factor because $\operatorname{Re}z>0$.

The $\gamma_1$ integral is analytic in $z$ because its contour is finite, and it is a nonzero solution. By uniqueness of the analytic local solution, it is a constant multiple of $y_1$. This is the [Finite Laguerre contour solution](../../../../../../finite-laguerre-contour-solution.md) construction.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
