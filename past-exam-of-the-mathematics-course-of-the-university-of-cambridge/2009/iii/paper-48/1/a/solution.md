<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [position eigenstates](../../../../../../position-eigenstate.md) normalized by $\langle q|q'\rangle=\delta(q-q')$, and the free [Hamiltonian operator](../../../../../../hamiltonian-quantum-mechanics.md) $\widehat H=\widehat p^2/(2m)$. The time-sliced [path integral](../../../../../../path-integral.md) is the matrix element of the [time-evolution operator](../../../../../../time-evolution-operator.md):

$$
\boxed{\mathcal I[q^{(i)},q^{(f)}]=\langle q^{(f)}|e^{-iT\widehat H/\hbar}|q^{(i)}\rangle.}
$$

Insert [momentum eigenstates](../../../../../../momentum-eigenstate.md), with $\langle q|p\rangle=(2\pi\hbar)^{-1/2}e^{ipq/\hbar}$. The [free-particle propagator](../../../../../../free-particle-propagator.md) becomes

$$
\mathcal I=\int_{-\infty}^{\infty}\frac{dp}{2\pi\hbar}\exp\!\left(\frac{ip\Delta q}{\hbar}-\frac{iTp^2}{2m\hbar}\right),\qquad\Delta q=q^{(f)}-q^{(i)}.
$$

Complete the square in the exponent:

$$
\frac{ip\Delta q}{\hbar}-\frac{iTp^2}{2m\hbar}=-\frac{iT}{2m\hbar}\left(p-\frac{m\Delta q}{T}\right)^2+\frac{im(\Delta q)^2}{2\hbar T}.
$$

The [Fresnel integral](../../../../../../fresnel-integral.md), defined by the damping prescription $T\to T-i0$, gives, for $T>0$,

$$
\boxed{\mathcal I=\left(\frac{m}{2\pi i\hbar T}\right)^{1/2}\exp\!\left(\frac{im(\Delta q)^2}{2\hbar T}\right).}
$$

The square-root branch is $i^{-1/2}=e^{-i\pi/4}$; it is fixed by the regulated [Gaussian integral](../../../../../../gaussian-integral.md) and the short-time [Dirac delta distribution](../../../../../../dirac-delta-function.md) limit, rather than an arbitrary phase.

The [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) for the [free particle](../../../../../../free-particle.md) is $m\ddot q=0$. Its unique classical path satisfying the endpoint [boundary conditions](../../../../../../boundary-condition.md) is $q_{\rm cl}(t)=q^{(i)}+\Delta q\,t/T$. Therefore its classical [action](../../../../../../action.md) is

$$
\boxed{S_{\rm cl}=\int_0^T\frac m2\left(\frac{\Delta q}{T}\right)^2dt=\frac{m(\Delta q)^2}{2T}.}
$$

Substituting into the operator result yields $\mathcal I=C(T)e^{iS_{\rm cl}/\hbar}$, with $C(T)=(m/(2\pi i\hbar T))^{1/2}$ independent of the endpoint positions.

The same independence is transparent directly in the [path integral](../../../../../../path-integral.md). Write $q=q_{\rm cl}+\eta$, with $\eta(0)=\eta(T)=0$. The cross term in the [action](../../../../../../action.md) is $m\dot q_{\rm cl}\int_0^T\dot\eta\,dt=0$, so $S[q]=S_{\rm cl}+(m/2)\int_0^T\dot\eta^2dt$. The fluctuation integral depends only on $m,T,\hbar$. Because the [action](../../../../../../action.md) is quadratic, the factorization is exact; the [semiclassical propagator](../../../../../../semiclassical-propagator.md) already equals the full answer.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
