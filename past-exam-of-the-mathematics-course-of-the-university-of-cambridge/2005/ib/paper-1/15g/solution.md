<h1 id="15g/solution">Solution</h1>

↑ **Parent:** [15G](../15g.md)

Inside the [infinite square well](../../../../../infinite-square-well.md), the time-independent [Schrödinger equation](../../../../../schrodinger-equation.md) is $-\hbar^2u''/(2m)=Eu$ with $u(-a)=u(a)=0$. For $E<0$ the exponential solutions cannot satisfy both conditions except trivially, and for $E=0$ neither can a linear function. For $E>0$ put $k=\sqrt{2mE}/\hbar$. The first boundary condition selects $u=C\sin(k(x+a))$, and the second gives $\sin(2ak)=0$. Thus

$$
\boxed{u_n(x)=\frac1{\sqrt a}\sin\!\left(\frac{n\pi(x+a)}{2a}\right),\qquad
E_n=\frac{\hbar^2\pi^2n^2}{8ma^2},\quad n=1,2,\ldots}
$$

on $[-a,a]$, with $u_n=0$ outside. Their squared integrals are one, and the sine [orthogonality](../../../../../orthogonal-vectors.md) identity gives an [orthonormal set](../../../../../orthonormal-set.md). The sine [Fourier basis](../../../../../fourier-basis.md) on the interval is complete: odd extension to an interval of length $4a$ reduces this to completeness of the [Fourier series](../../../../../fourier-series-split.md) basis. Hence these are a complete set of normalized [energy eigenstates](../../../../../energy-eigenstate.md).

Choosing the harmless sign of the second [energy eigenstate](../../../../../energy-eigenstate.md) so that $v_1=a^{-1/2}\cos(\pi x/(2a))$ and $v_2=a^{-1/2}\sin(\pi x/a)$, the specified [wave function](../../../../../wave-function.md) is $v_1/\sqrt5+2v_2/\sqrt5$. The [Born rule](../../../../../born-rule.md) therefore gives

$$
\boxed{\Pr(E=E_1)=\frac15,\qquad\Pr(E=E_2)=\frac45},
$$

with no other possible measured energies. The two [energy eigenvalues](../../../../../energy-eigenvalue.md) are $E_1=\hbar^2\pi^2/(8ma^2)$ and $E_2=4E_1$.

After the first measurement gives the [ground state](../../../../../ground-state.md), the old state is $v_1$. Doubling the width puts the walls at $\pm2a$, and the new normalized [ground state](../../../../../ground-state.md) is $w_1=(2a)^{-1/2}\cos(\pi x/(4a))$. The stipulated unchanged state is zero outside the original interval, so the [probability amplitude](../../../../../probability-amplitude.md) is

$$
\langle w_1,v_1\rangle
=\frac1{\sqrt2\,a}\int_{-a}^a
\cos\!\left(\frac{\pi x}{4a}\right)\cos\!\left(\frac{\pi x}{2a}\right)\,dx
=\frac8{3\pi}.
$$

Squaring gives

$$
\boxed{\Pr(\text{new ground state}\mid\text{old ground state})=\frac{64}{9\pi^2}}.
$$

The [ground-state overlap after sudden expansion of a square well](../../../../../ground-state-overlap-after-sudden-expansion-of-a-square-well.md) stays unchanged during subsequent evolution in the fixed new well, because the energy-basis coefficients acquire only phases. The answer is conditional on the already observed old [ground state](../../../../../ground-state.md); its earlier probability $1/5$ is not another factor in this conditional question.

## ↑ Ancestors (10)

1. [15G](../15g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
