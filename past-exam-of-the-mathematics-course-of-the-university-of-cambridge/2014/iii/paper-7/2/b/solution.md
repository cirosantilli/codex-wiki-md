<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix the mixed [Fourier transform](../../../../../../fourier-transform.md) convention

$$
 \widehat f(t,k,\xi)=\int_0^1\int_{\mathbb R}
 f(t,x,v)e^{-2\pi i(kx+\xi v)}\,dv\,dx,
 \qquad k\in\mathbb Z,\quad\xi\in\mathbb R.
$$

The spatial derivative transforms to $2\pi ik\widehat f$, and multiplication by $v$ transforms to $-(2\pi i)^{-1}\partial_\xi\widehat f$. Hence the transformed [free transport equation](../../../../../../free-transport-equation.md) is

$$
 \boxed{\partial_t\widehat f-k\partial_\xi\widehat f=0.}
$$

Its [characteristic equations for a transport equation](../../../../../../characteristic-equations-for-a-transport-equation.md) give $\dot\xi=-k$, so the characteristic ending at $\xi$ at time $t$ began at $\xi+kt$. Consequently

$$
 \boxed{\widehat f(t,k,\xi)=\widehat f_0(k,\xi+kt).}
$$

The same sign follows directly by substituting $x=y+tv$ in the [Fourier transform](../../../../../../fourier-transform.md) of $f_0(x-tv,v)$. No first velocity moment is assumed, so the differential equation may be understood in the sense of [tempered distributions](../../../../../../tempered-distribution.md); the explicit transform formula is valid pointwise because $f_0$ is integrable.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
