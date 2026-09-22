<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

For an endpoint-fixed variation $\eta=\delta x$,

$$
\delta S=\int_0^T(\dot x\dot\eta-\omega^2x\eta)dt
=[\dot x\eta]_0^T-\int_0^T(\ddot x+\omega^2x)\eta\,dt.
$$

The boundary term vanishes. Thus every solution of the [harmonic oscillator equation](../../../../../simple-harmonic-motion.md) is stationary for this [action functional](../../../../../action.md). For $\sin\omega T\ne0$, the endpoint-matching solution is the linear combination

$$
x_c(t)=\frac{a\sin\omega(T-t)+b\sin\omega t}{\sin\omega T},
$$

which directly satisfies $x_c(0)=a$, $x_c(T)=b$ and $\ddot x_c=-\omega^2x_c$. This proves stationarity, rather than assuming the explicit path is a minimum.

On that path, $(x_c\dot x_c)'=\dot x_c^2-\omega^2x_c^2$, so [integration by parts](../../../../../integration-by-parts.md) reduces the entire action to an endpoint term. The endpoint derivatives are

$$
\dot x_c(0)=\frac{\omega(b-a\cos\omega T)}{\sin\omega T},\qquad
\dot x_c(T)=\frac{\omega(b\cos\omega T-a)}{\sin\omega T}.
$$

Therefore the [fixed-endpoint harmonic-oscillator action](../../../../../fixed-endpoint-harmonic-oscillator-action.md) is

$$
\boxed{S[x_c]=\left[\frac12x_c\dot x_c\right]_0^T
=\frac{\omega}{2\sin\omega T}\bigl[(a^2+b^2)\cos\omega T-2ab\bigr].}
$$

The displayed formula assumes nonresonant endpoints. If $\omega\ne0$ and $\omega T=k\pi$, a solution exists only for $b=(-1)^ka$; then $x=a\cos\omega t+B\sin\omega t$ is a family and its action is zero. For $\omega=0$ the limiting stationary path is linear, with action $(b-a)^2/(2T)$.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
