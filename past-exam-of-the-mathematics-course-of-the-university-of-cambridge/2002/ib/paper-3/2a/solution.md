<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

Let the mass per unit length be $m$ and the constant tension be $T$. Small transverse displacement obeys the [wave equation](../../../../../wave-equation-split.md)

$$
\boxed{m y_{tt}=T y_{xx},\qquad y_{tt}=c^2y_{xx},\quad c=\sqrt{T/m}}.
$$

With characteristic coordinates $\xi=x+ct$ and $\eta=x-ct$, the equation becomes $y_{\xi\eta}=0$. Integrating once in each variable gives [D'Alembert's formula](../../../../../d-alembert-s-formula.md)

$$
\boxed{y(x,t)=f(x+ct)+g(x-ct)}.
$$

For a smooth solution with vanishing endpoint [energy](../../../../../energy.md) flux, multiplication by $y_t$ and integration by parts give

$$
\frac{dE}{dt}=\int_0^\infty y_t(y_{tt}-c^2y_{xx})\,dx+[c^2y_ty_x]_0^\infty=0.
$$

The fixed endpoint has $y_t(0,t)=0$. Decay of displacement alone does not guarantee either a pointwise derivative-flux limit or finiteness of the [energy](../../../../../energy.md) integral; the conservation statement is understood in the usual finite-[energy](../../../../../energy.md) class. The profile formula below proves it directly there without requiring such a pointwise limit at infinity.

The endpoint condition gives $g(-ct)=-f(ct)$, allowing the reflected wave to be expressed through one profile:

$$
y(x,t)=f(x+ct)-f(ct-x).
$$

For forward time one may define the negative-argument part of this profile using the original $g$; no restriction on the independent initial waves is lost. Differentiation gives $y_t=c[f'(x+ct)-f'(ct-x)]$ and $y_x=f'(x+ct)+f'(ct-x)$. Hence

$$
\boxed{E=c^2\int_0^\infty\bigl[f'(x+ct)^2+f'(ct-x)^2\bigr]dx
=c^2\int_{-\infty}^{\infty}f'(s)^2\,ds}.
$$

The two substitutions partition the real line at $ct$, making [conservation of energy](../../../../../conservation-of-energy.md) explicit.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
