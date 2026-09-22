<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\kappa>0$, divide the [Boundary-point Bessel flow for SLE](../../../../../../boundary-point-bessel-flow-for-sle.md) by $\sqrt\kappa$ and replace $W$ by $-W$. The resulting [Bessel process](../../../../../../bessel-process.md) has dimension

$$
\delta=1+\frac4\kappa,
$$

since its drift is $\tfrac{\delta-1}{2R_t}=2/(\kappa R_t)$. The [Hitting-zero classification for a Bessel process](../../../../../../hitting-zero-classification-for-a-bessel-process.md) suggests the threshold $\delta=2$, or $\kappa=4$. Here is a direct verification including accessibility in finite time.

The [infinitesimal generator](../../../../../../infinitesimal-generator-stochastic-processes.md) of $X$ is $\mathcal L=\tfrac\kappa2\partial_x^2+(2/x)\partial_x$. An increasing [scale function of a one-dimensional diffusion](../../../../../../scale-function-stochastic-processes.md) is

$$
s(x)=\begin{cases}
\dfrac{x^{1-4/\kappa}}{1-4/\kappa},&\kappa\ne4,\\
\log x,&\kappa=4.
\end{cases}
$$

It satisfies $\mathcal Ls=0$. For $0<\varepsilon<b<R$, the [boundary hitting probability from a diffusion scale function](../../../../../../boundary-hitting-probability-from-a-diffusion-scale-function.md), or [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) applied to $s(X)$, gives

$$
\mathbb P_b(T_\varepsilon<T_R)
=\frac{s(R)-s(b)}{s(R)-s(\varepsilon)}.
$$

For $0<\kappa<4$, $s(\varepsilon)\to-\infty$, so this probability tends to zero as $\varepsilon\downarrow0$. A finite zero hit has a bounded path before the hit and hence precedes $T_R$ for some integer $R$; taking a countable union proves that zero is never hit.

For $\kappa>4$, write $a=1-4/\kappa>0$. Taking the inner boundary to zero gives $1-(b/R)^a$. This limit really concerns a finite zero hit: the [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
d(X_t^2)=(\kappa+4)dt-2\sqrt\kappa X_t\,dW_t.
$$

Stopped on $[\varepsilon,R]$, it implies

$$
\mathbb E_b(T_\varepsilon\wedge T_R)
\leq\frac{R^2-b^2}{\kappa+4},
$$

uniformly in $\varepsilon$. The increasing limit of these exit times is finite [almost surely](../../../../../../almost-sure-convergence.md); the stopped squared process has a continuous extension, so its limiting lower endpoint is zero. Thus

$$
\mathbb P_b(T_0<T_R)=1-(b/R)^a.
$$

Let $R\to\infty$ to obtain $\mathbb P_b(T_0<\infty)=1$. When $\kappa=0$, the explicit solution is $X_t=\sqrt{b^2+4t}$, which stays positive.

Combining this with the [SLE boundary swallowing criterion](../../../../../../sle-boundary-swallowing-criterion.md) gives **the critical parameter and the two regimes**:

$$
\boxed{\kappa_c=4,\qquad
\mathbb P(\gamma\text{ hits }[b,\infty))=
\begin{cases}0,&0\leq\kappa<4,\\1,&\kappa>4.\end{cases}}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
