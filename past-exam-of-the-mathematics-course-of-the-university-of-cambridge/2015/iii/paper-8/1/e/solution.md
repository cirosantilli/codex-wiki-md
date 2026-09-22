<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For the [isotropic harmonic oscillator flow](../../../../../../isotropic-harmonic-oscillator-flow.md), [Hamilton's equations](../../../../../../hamilton-s-equations.md) are $\dot X=V$, $\dot V=-\omega^2X$. In dimension three these are three identical uncoupled pairs. For $\omega\ne0$, put $c_t=\cos(\omega t)$, $s_t=\sin(\omega t)$. The solution from $(x,v)$ at time zero is

$$
\boxed{X(t)=c_tx+\frac{s_t}{\omega}v,\qquad
V(t)=-\omega s_tx+c_tv.}
$$

The inverse flow is obtained by replacing $t$ by $-t$:

$$
S_{-t}(x,v)=\left(c_tx-\frac{s_t}{\omega}v,\ \omega s_tx+c_tv\right).
$$

Integrating the source along the backward characteristic gives the [Duhamel formula for Hamiltonian transport](../../../../../../duhamel-formula-for-hamiltonian-transport.md):

$$
\boxed{f(t,x,v)=
f_0\!\left(c_tx-\frac{s_t}{\omega}v,\ \omega s_tx+c_tv\right)
+\int_0^t h\!\left(s,\ c_{t-s}x-\frac{s_{t-s}}{\omega}v,\
\omega s_{t-s}x+c_{t-s}v\right)\,ds.}
$$

Indeed $f(t,S_tz)=f_0(z)+\int_0^th(s,S_sz)\,ds$, and setting $z=S_{-t}(x,v)$ gives the formula. It has the prescribed initial value and differentiation along the characteristic gives the source.

The zero-frequency limit has $s_t/\omega\to t$, $\omega s_t\to0$, so $S_t(x,v)=(x+tv,v)$ and

$$
\boxed{f(t,x,v)=f_0(x-tv,v)+\int_0^th(s,x-v(t-s),v)\,ds\qquad(\omega=0).}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
