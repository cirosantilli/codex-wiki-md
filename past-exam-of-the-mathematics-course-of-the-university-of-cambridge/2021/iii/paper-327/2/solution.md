<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [phase function](../../../../../phase-function.md) is a real smooth function

$$
\Phi:X\times(\mathbb R^k\setminus\{0\})\to\mathbb R
$$

that is [positively homogeneous](../../../../../positively-homogeneous-function-degree-one.md) of degree one in $\theta$ and has no critical point in all variables:

$$
\Phi(x,t\theta)=t\Phi(x,\theta),
\qquad
\nabla_{x,\theta}\Phi(x,\theta)\ne0.
$$

The [symbol class](../../../../../symbol-class.md) $\operatorname{Sym}(X,\mathbb R^k;N)$ consists of all $a\in C^\infty(X\times\mathbb R^k)$ such that, for every compact $K\Subset X$ and [multi-indices](../../../../../multi-index-notation.md) $\alpha,\beta$,

$$
|D_x^\alpha D_\theta^\beta a(x,\theta)|
\leq C_{K,\alpha,\beta}(1+|\theta|)^{N-|\beta|}.
$$

For a cutoff $\chi\in C_c^\infty(\mathbb R^k)$ equal to one near zero, define the [oscillatory integral](../../../../../oscillatory-integral.md) by

$$
\boxed{
\langle I_\Phi(a),\psi\rangle
=\lim_{\varepsilon\downarrow0}
\int_X\int_{\mathbb R^k}
e^{i\Phi(x,\theta)}a(x,\theta)\psi(x)\chi(\varepsilon\theta)
\,d\theta\,dx}.
$$

Repeated [integration by parts](../../../../../integration-by-parts.md) makes the limit meaningful and independent of the cutoff.

The [singular support](../../../../../singular-support.md) is the complement of the largest open set on which the distribution is represented by a [smooth function](../../../../../smooth-function.md). Suppose $x_0$ does not belong to

$$
C_\Phi=\{x:\nabla_\theta\Phi(x,\theta)=0
\text{ for some }\theta\ne0\}.
$$

On a sufficiently small neighborhood of $x_0$, homogeneity and compactness of the unit sphere give a lower bound for $|\nabla_\theta\Phi|$. The differential operator

$$
L=\frac{\nabla_\theta\Phi\mathbin\cdot\nabla_\theta}
{i|\nabla_\theta\Phi|^2}
$$

satisfies $Le^{i\Phi}=e^{i\Phi}$. Repeatedly transferring $L$ to the amplitude lowers its symbol order until the integral and all its $x$-derivatives converge absolutely. Hence $I_\Phi(a)$ is smooth near $x_0$, proving

$$
\boxed{\operatorname{sing\,supp}I_\Phi(a)\subseteq C_\Phi}.
$$

For the stated distribution on $\mathbb R^3$, rotational symmetry lets us align the polar axis with $x$ and write $\rho=|x|$. The angular integral is

$$
\int_0^{2\pi}\int_0^\pi
e^{ir\rho\cos\theta}\sin\theta\,d\theta\,d\phi
=4\pi\frac{\sin(r\rho)}{r\rho}.
$$

Therefore, for $\rho>0$,

$$
\begin{aligned}
u(x)
&=\frac1{2\pi}\frac{4\pi}{\rho}
\int_0^\infty\frac{r\sin(r\rho)}{1+r^2}\,dr\\
&=\boxed{\frac{\pi e^{-\rho}}{\rho}}.
\end{aligned}
$$

The original amplitude is not [Lebesgue integrable](../../../../../lebesgue-integrable-function.md) in $k$, so this computation illustrates how oscillation assigns a distribution to a divergent ordinary integral. The result is smooth away from the origin and has singular support $\{0\}$. It is a constant multiple of the three-dimensional [Yukawa potential](../../../../../yukawa-potential.md), satisfying $(-\Delta+1)u=4\pi^2\delta_0$ with the normalization used in the question.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 327](../../paper-327-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
