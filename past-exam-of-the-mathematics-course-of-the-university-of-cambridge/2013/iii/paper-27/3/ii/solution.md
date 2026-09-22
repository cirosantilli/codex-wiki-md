<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $\kappa>0$ and $x\ne0$, since the initial driving point does not admit the displayed ordinary boundary flow. The sign of the driver in this part is negative, so

$$
d\bigl(g_t(x\sqrt\kappa)-\xi_t\bigr)
=\frac2{g_t(x\sqrt\kappa)-\xi_t}\,dt+\sqrt\kappa\,dW_t.
$$

After division by $\sqrt\kappa$, the [Boundary-point Bessel flow for SLE](../../../../../../boundary-point-bessel-flow-for-sle.md) is

$$
\boxed{dX_t=dW_t+\frac a{X_t}\,dt,\qquad
X_0=x,\qquad a=\frac2\kappa.}
$$

For $x>0$ this is a [Bessel process](../../../../../../bessel-process.md) of dimension $\delta=1+2a$. For $x<0$, $-X_t$ obeys the same equation driven by $-W_t$ until hitting zero. It suffices to treat a positive initial value.

The [infinitesimal generator](../../../../../../infinitesimal-generator-stochastic-processes.md) is $\mathcal Lf=\tfrac12f''+(a/u)f'$. An increasing [scale function of a one-dimensional diffusion](../../../../../../scale-function-stochastic-processes.md) is

$$
s(u)=
\begin{cases}
u^{1-2a}/(1-2a),&a\ne1/2,\\
\log u,&a=1/2.
\end{cases}
$$

It satisfies $\mathcal Ls=0$. For $0<\varepsilon<x<b$, [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives the [boundary hitting probability from a diffusion scale function](../../../../../../boundary-hitting-probability-from-a-diffusion-scale-function.md)

$$
\mathbb P_x(\tau_\varepsilon<\tau_b)
=\frac{s(b)-s(x)}{s(b)-s(\varepsilon)}.
$$

When $a<1/2$, put $\beta=1-2a>0$. The inner boundary is reached in finite time: the nonnegative function

$$
v(u)=\frac{b^{2-\beta}u^\beta-u^2}{1+2a}
$$

vanishes at $0,b$ and satisfies $\mathcal Lv=-1$. Applying the [Itô formula](../../../../../../ito-s-lemma.md) before exiting $(\varepsilon,b)$ gives $\mathbb E(\tau_\varepsilon\wedge\tau_b)\le v(x)$. As $\varepsilon\downarrow0$, these times increase to a finite limiting exit time almost surely. Thus the scale limit is an actual hitting event, not just asymptotic approach to zero, and

$$
\mathbb P_x(\tau_0<\tau_b)=1-(x/b)^\beta.
$$

Let $b\uparrow\infty$ to obtain $\mathbb P_x(\tau_0<\infty)=1$.

If $a>1/2$, then $s(\varepsilon)\to-\infty$, and the same formula makes the probability of hitting zero before any fixed $b$ equal to zero. A finite-time hit would occur before reaching some integer upper level, because the stopped path is continuous and bounded on a finite interval. Taking the countable union over those levels proves that no hit occurs. At $a=1/2$, $s(u)=\log u$ gives the same conclusion. Therefore

$$
\boxed{\tau_0<\infty\text{ a.s. if }a<\tfrac12;\qquad
\tau_0=\infty\text{ a.s. if }a\ge\tfrac12.}
$$

The source's $x=0$ case must be excluded: zero is then already the initial value, and the displayed singular flow is undefined.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
