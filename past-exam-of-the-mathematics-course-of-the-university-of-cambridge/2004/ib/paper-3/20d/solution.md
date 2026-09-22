<h1 id="20d/solution">Solution</h1>

↑ **Parent:** [20D](../20d.md)

The scattering interpretation assumes $0<\epsilon<U$, so $k=\sqrt\epsilon$ is real and $K=\sqrt{U-\epsilon}>0$. The incoming amplitudes are $a$ from the left and $b$ from the right; the outgoing amplitudes are $c,d$. The conserved [probability current](../../../../../probability-current.md) is

$$
j=\frac\hbar m\operatorname{Im}(\psi^*\psi'),
$$

which gives $j=\hbar k(|a|^2-|c|^2)/m$ on the left and $j=\hbar k(|d|^2-|b|^2)/m$ on the right. Equality proves **$|c|^2+|d|^2=|a|^2+|b|^2$**. Equal exterior wavenumbers make the flux weights equal.

Continuity of the [wavefunction](../../../../../wave-function.md) and its derivative at the finite potential steps yields the four relations, with $C=\cosh KL$ and $S=\sinh KL$,

$$
a+c=e,\qquad ik(a-c)=Kf,\qquad
d+b=eC+fS,\qquad ik(d-b)=K(eS+fC).
$$

Set $\lambda=K/(ik)$. Substituting $e=a+c$, $f=(a-c)/\lambda$ and subtracting the last two relations after dividing the fourth by $ik$ gives

$$
2b=2cC+\left[\frac{a-c}{\lambda}-\lambda(a+c)\right]S
=2Dc-(\lambda-\lambda^{-1})Sa,
$$

where $D=C-(\lambda+\lambda^{-1})S/2$. Hence

$$
\boxed{c=\frac{b+\tfrac12(\lambda-\lambda^{-1})Sa}{D}.}
$$

Reflection about the barrier midpoint interchanges the left and right incidence problems and, with the chosen phase origins, exchanges $a\leftrightarrow b$ and $c\leftrightarrow d$. Therefore

$$
\boxed{d=\frac{a+\tfrac12(\lambda-\lambda^{-1})Sb}{D}.}
$$

For incidence from the left alone, the [transmission coefficient](../../../../../transmission-coefficient.md) is the transmitted-to-incident probability flux ratio, $T=|d/a|^2=|D|^{-2}$. Since $\lambda=-iK/k$, direct calculation gives

$$
|D|^2=1+\frac{(K^2+k^2)^2}{4k^2K^2}\sinh^2KL
=1+\frac{U^2}{4\epsilon(U-\epsilon)}\sinh^2KL.
$$

For fixed energy inside the barrier range and $KL\gg1$, $\sinh^2KL\sim e^{2KL}/4$, so

$$
\boxed{T\sim16\frac{\epsilon(U-\epsilon)}{U^2}e^{-2\sqrt{U-\epsilon}\,L}.}
$$

This is the thick-barrier [quantum tunnelling](../../../../../quantum-tunnelling.md) limit, not a uniform approximation as energy approaches the barrier top while $KL$ remains small.

## ↑ Ancestors (10)

1. [20D](../20d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
