<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The positive uniform ellipticity condition from part (i) is needed here. It is not explicitly imposed in the printed preamble. Without it the conclusion is false: on $(0,\pi)$, take $L=u''$, $\beta=0$, and $f=0$. The [Neumann boundary condition](../../../../../../../neumann-boundary-condition.md) is satisfied by $u(x)=\cos(mx)$, and $(L+m^2)u=0$ for arbitrarily large shifts.

There is also an actual error in the PDF's supplied trace inequality: a nonzero constant has nonzero trace and zero gradient. Use instead the valid [multiplicative trace inequality on a bounded smooth domain](../../../../../../../multiplicative-trace-inequality-on-a-bounded-smooth-domain.md)

$$
\|Tu\|_{L^2(\partial U)}^2\leq K\bigl(\|u\|_2\|Du\|_2+\|u\|_2^2\bigr).
$$

For completeness, choose a smooth vector field $X$ agreeing with the outward [normal vector](../../../../../../../normal-vector.md) on the boundary. The [divergence theorem](../../../../../../../divergence-theorem.md) gives, for smooth $u$,

$$
\int_{\partial U}u^2dS
=\int_U(\operatorname{div}X)u^2+2uX\cdot Du\,dx
\leq C\bigl(\|u\|_2^2+\|u\|_2\|Du\|_2\bigr).
$$

Approximation and the [Sobolev trace theorem](../../../../../../../sobolev-trace-theorem.md) extend it to $H^1(U)$. Thus the intended existence result remains true after correcting the hint.

Set $q=\|u\|_2$, $d=\|Du\|_2$, $\beta_- =\max\{-\beta,0\}$, $c_- =\max\{-c,0\}$, and

$$
M=\|b\|_\infty+K\|\beta_-\|_\infty,\qquad
C_0=\|c_-\|_\infty+K\|\beta_-\|_\infty+\frac{M^2}{2\theta}.
$$

Uniform ellipticity and the [Young inequality](../../../../../../../young-s-inequality-for-products.md) give

$$
\begin{aligned}
B_\lambda[u,u]
&\geq\theta d^2-Mqd+
(\lambda-\|c_-\|_\infty-K\|\beta_-\|_\infty)q^2\\
&\geq\frac\theta2d^2+(\lambda-C_0)q^2.
\end{aligned}
$$

For $\lambda\geq C_0+1$, the [bilinear form](../../../../../../../bilinear-form.md) is [coercive](../../../../../../../coercive-bilinear-form.md) on the real [Hilbert space](../../../../../../../hilbert-space-split.md) $H^1(U)$ with coercivity constant $\min\{\theta/2,1\}$.

All coefficients are bounded, and the [Sobolev trace theorem](../../../../../../../sobolev-trace-theorem.md) gives $\|Tu\|_2\leq C_T\|u\|_{H^1}$. The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) applied to each volume and boundary term therefore proves $|B_\lambda[u,v]|\leq C_\lambda\|u\|_{H^1}\|v\|_{H^1}$. Also $\ell(v)=\int_Ufv$ is a [continuous linear functional](../../../../../../../continuous-linear-functional.md), with $|\ell(v)|\leq\|f\|_2\|v\|_{H^1}$. Every hypothesis of the [Lax-Milgram theorem](../../../../../../../lax-milgram-theorem.md) is now verified, and it gives

$$
\boxed{\text{a unique }u\in H^1(U)\text{ for every }f\in L^2(U),
\quad\lambda\geq C_0+1,\quad
\|u\|_{H^1}\leq\frac{\|f\|_2}{\min\{\theta/2,1\}}.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
