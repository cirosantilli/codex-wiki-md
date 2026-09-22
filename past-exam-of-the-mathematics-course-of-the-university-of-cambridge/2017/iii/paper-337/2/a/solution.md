<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $R^2=1-q^2>0$. The symbol $R$ in this part is the [convection roll](../../../../../../convection-roll.md) amplitude, not the [Rayleigh number](../../../../../../rayleigh-number.md) of the previous part. Set $r=R^2$ for the algebra. The [periodic boundary condition](../../../../../../periodic-boundary-conditions.md) requires $qL\in2\pi\mathbb Z$ and modulation [wavenumbers](../../../../../../wavenumber.md) $lL\in2\pi\mathbb Z$. The conserved-field equation preserves the imposed zero mean of $B$, since the integral of an $X$ derivative over a period vanishes.

Equating the $e^{ilX+\lambda T}$ coefficients after [linearization](../../../../../../linearization.md) of the [convection amplitude coupled to a conserved field](../../../../../../convection-amplitude-coupled-to-a-conserved-field.md) gives

$$
\begin{aligned}\lambda a_1&=-(l^2+2ql)a_1-r(a_1+a_2)-b,\\\lambda a_2&=-(l^2-2ql)a_2-r(a_1+a_2)-b,\\\lambda b&=-\sigma l^2b-\mu r l^2(a_1+a_2).\end{aligned}
$$

The conjugate sideband is needed because the variation of $|A|^2A$ couples a perturbation to its [complex conjugate](../../../../../../complex-conjugate.md). Put $S=a_1+a_2$, $D=a_1-a_2$. The [linear operator](../../../../../../linear-operator.md) on $(S,D,b)$ is

$$
M_l=\begin{pmatrix}-l^2-2r&-2ql&-2\\-2ql&-l^2&0\\-\mu r l^2&0&-\sigma l^2\end{pmatrix}.
$$

Its [characteristic polynomial](../../../../../../characteristic-polynomial.md), expressed conveniently without expanding every coefficient, is

$$
\boxed{(\lambda+\sigma l^2)\big[(\lambda+l^2)(\lambda+l^2+2r)-4q^2l^2\big]-2\mu r l^2(\lambda+l^2)=0.}
$$

At $l=0$ it has roots $-2r,0,0$. The phase root is neutral; the uniform $B$ root is excluded by the prescribed zero-flux-perturbation mean. Nonzero arbitrarily long-wave modes remain allowed on a sufficiently large domain. For fixed $r>0$, the two roots tending to zero have $\lambda=l^2\nu+O(l^4)$ at simple limiting roots. Dividing the polynomial by $2l^4$ yields

$$
\boxed{r\nu^2-[(\mu-\sigma-1)r+2q^2]\nu-[(\mu-\sigma)r+2\sigma q^2]=0.}
$$

Repeated limiting roots may require a further expansion, but do not affect the strict instability criterion. If $(\mu-\sigma)r+2\sigma q^2>0$, the constant term is negative and the two real roots have opposite signs. The positive root gives a growing long-wave [sideband instability](../../../../../../sideband-instability.md). Using $r=1-q^2$ gives

$$
\boxed{\frac\mu\sigma>\frac{1-3q^2}{1-q^2}.}
$$

This is sufficient for instability when a sufficiently small nonzero allowed $l$ is available. It is not an unconditional instability theorem for every fixed finite period. For example $q=0$, $\mu=2$, $\sigma=1$, $L=1$ satisfy the inequality, but the nonzero allowed $l$ obey $l^2\geq4\pi^2$. Their roots are $-l^2$ and $-l^2-1\pm\sqrt{1+4l^2}$, all negative. The prescribed zero mean removes the uniform flux root and the remaining uniform phase is merely neutral. The corrected conclusion is the [long-wave instability with a conserved mean field](../../../../../../long-wave-instability-with-a-conserved-mean-field.md), with domain size and mode availability stated.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
