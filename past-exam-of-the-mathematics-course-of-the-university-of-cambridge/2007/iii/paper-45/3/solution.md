<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The surplus in the [classical risk model](../../../../../classical-risk-model.md) is $U(t)=u+ct-S(t)$. With ruin defined as a strictly negative surplus, its [ultimate ruin probability](../../../../../ultimate-ruin-probability.md) is

$$
\boxed{\psi(u)=\mathbb P\{U(t)<0\text{ for some }t\geq0\}
=\mathbb P\{S(t)-ct>u\text{ for some }t\geq0\}.}
$$

Let $\overline F_X(v)=\int_v^\infty f_X(x)\,dx$. The first arrival time has [exponential distribution](../../../../../exponential-distribution.md) of rate $\lambda$, independent of the first claim. Before that claim no ruin occurs, because the premium rate is positive. Given its arrival at $t$ and size $x$, available capital just before it is $u+ct$. If $x>u+ct$ ruin is immediate; otherwise the [independent increments](../../../../../independent-increments.md) and fresh claim sizes make subsequent ruin probability $\psi(u+ct-x)$. Thus first-claim conditioning gives

$$
\psi(u)=\int_0^\infty\lambda e^{-\lambda t}\left[
\overline F_X(u+ct)+\int_0^{u+ct}f_X(x)\psi(u+ct-x)\,dx\right]dt.
$$

This is the ruin counterpart of the [first-claim decomposition for survival probability](../../../../../first-claim-decomposition-for-survival-probability.md). Define

$$
H(v)=\overline F_X(v)+\int_0^v f_X(x)\psi(v-x)\,dx.
$$

The [convolution](../../../../../convolution.md) term is continuous: extend the bounded function $\psi$ by zero to negative arguments and use continuity of translations in $L^1$ for the integrable density $f_X$. The tail function is also continuous. Changing variables to $v=u+ct$ yields

$$
\psi(u)=\frac\lambda c e^{\lambda u/c}\int_u^\infty e^{-\lambda v/c}H(v)\,dv.
$$

Differentiating this exponentially weighted integral establishes differentiability rather than presuming it. The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) gives

$$
\psi'(u)=\frac\lambda c\psi(u)-\frac\lambda c H(u).
$$

Reversing the integration variable in the convolution therefore proves the [ruin integro-differential equation](../../../../../ruin-integro-differential-equation.md):

$$
\boxed{\frac c\lambda\psi'(u)=\psi(u)-\int_0^u f_X(u-x)\psi(x)\,dx-\int_u^\infty f_X(x)\,dx.}
$$

At zero the derivative is the right derivative; the same representation supplies it.

For the exponential claim law, introduce

$$
A(u)=\int_0^u\alpha e^{-\alpha(u-x)}\psi(x)\,dx,
\qquad H(u)=A(u)+e^{-\alpha u}.
$$

Differentiating the explicit convolution gives $A'=\alpha\psi-\alpha A$. Hence

$$
H'(u)=\alpha\psi(u)-\alpha H(u)
=\frac{\alpha c}{\lambda}\psi'(u),
$$

using the proved integral equation. Differentiating that equation once more gives

$$
\frac c\lambda\psi''=\psi'-H'
=\left(1-\frac{\alpha c}{\lambda}\right)\psi',
$$

so the required [ordinary differential equation](../../../../../ordinary-differential-equation.md) is

$$
\boxed{\psi''(u)+\left(\alpha-\frac\lambda c\right)\psi'(u)=0.}
$$

Positive [relative safety loading](../../../../../relative-safety-loading.md) means $c>\lambda/\alpha$, so $\kappa=\alpha-\lambda/c>0$. The general solution is $a+b e^{-\kappa u}$.

The condition at large capital must also be used. The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) for the [Poisson process](../../../../../poisson-process.md) and the independent claims gives $S(t)/t\to\lambda/\alpha$ almost surely. Thus $S(t)-ct\to-\infty$. Its path has only finitely many jumps on each bounded time interval, so its supremum over all time is finite almost surely. Therefore $\psi(u)\to0$ as $u\to\infty$, forcing $a=0$. The supplied initial value $\psi(0)=\lambda/(\alpha c)$ then gives [ultimate ruin with exponential claims](../../../../../ultimate-ruin-with-exponential-claims.md):

$$
\boxed{\psi(u)=\frac\lambda{\alpha c}\exp\left[-\left(\alpha-\frac\lambda c\right)u\right],\qquad u\geq0.}
$$

The decay rate is also the exponential-claim [adjustment coefficient](../../../../../adjustment-coefficient.md).

For the [maximum aggregate loss in a classical risk model](../../../../../maximum-aggregate-loss-in-a-classical-risk-model.md), the ruin event is exactly $\{L>u\}$. Since $L(0)=0$, $L\geq0$, and its full [cumulative distribution function](../../../../../cumulative-distribution-function.md) is

$$
\boxed{\mathbb P(L\leq u)=
\begin{cases}
0,&u<0,\\
1-\dfrac\lambda{\alpha c}e^{-\kappa u},&u\geq0.
\end{cases}}
$$

In particular it has an atom of mass $1-\lambda/(\alpha c)$ at zero. Conditional on $L>0$, its distribution is exponential with rate $\kappa$; omitting that atom would give an incorrectly normalized law.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
