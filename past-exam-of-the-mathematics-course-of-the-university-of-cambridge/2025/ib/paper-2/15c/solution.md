<h1 id="15c/solution">Solution</h1>

↑ **Parent:** [15C](../15c.md)

The commutator follows directly on a test [function](../../../../../function-split.md):

$$
[f,p]=i\hbar f'.
$$

Expansion gives

$$
V_+=\frac{f^2-\hbar f'}{2m},\qquad V_-=\frac{f^2+\hbar f'}{2m}.
$$

To make $V_-=2m$, take

$$
f(x)=2m\tanh(2mx/\hbar).
$$

Then

$$
V_+(x)=2m-4m\operatorname{sech}^2(2mx/\hbar),
$$

which tends to $2m$ at both ends.

Applying $p+if$ to $e^{ikx}$ gives a partner scattering state with asymptotic amplitudes $\hbar k-2mi$ at $-\infty$ and $\hbar k+2mi$ at $+\infty$, and no reflected wave. Their [moduli](../../../../../modulus.md) agree. Subtracting the common constant $2m$ therefore shows that the displayed $-4m\operatorname{sech}^2$ potential is reflectionless:

$$
\boxed{\mathcal R=0,\qquad \mathcal T=1.}
$$

## ↑ Ancestors (10)

1. [15C](../15c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
