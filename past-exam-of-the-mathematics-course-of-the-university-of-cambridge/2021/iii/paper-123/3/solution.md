<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Schwartz-Bruhat space](../../../../../schwartz-bruhat-space.md) $\mathcal S(F)$ of a non-Archimedean [local field](../../../../../local-field.md) $F$ is the vector space of locally constant, compactly supported complex-valued functions on $F$. Fix a nontrivial continuous [additive character](../../../../../additive-character.md) $\psi:F\to\mathbb C^\times$ and a [Haar measure](../../../../../haar-measure.md) $dx$. With the sign convention required in the question, the [Fourier transform over a local field](../../../../../fourier-transform-over-a-local-field.md) is

$$
\widehat f(y)=\int_F f(x)\psi(xy)\,dx.
$$

Let

$$
\mathcal O_F^\perp=\{y\in F:\psi(xy)=1\text{ for every }x\in\mathcal O_F\}
$$

be the [annihilator of the valuation ring](../../../../../annihilator-of-the-valuation-ring.md). Translation invariance gives

$$
\widehat{\mathbf1_{\mathcal O_F}}(y)
=\int_{\mathcal O_F}\psi(xy)\,dx
=\operatorname{vol}(\mathcal O_F)\mathbf1_{\mathcal O_F^\perp}(y).
$$

Indeed, the integral is the volume when the character is trivial; otherwise translation by an element on which the character is nontrivial multiplies the integral by a scalar different from one, forcing it to vanish. With the usual character of conductor $\mathcal O_F$ and the normalization $\operatorname{vol}(\mathcal O_F)=1$, this becomes

$$
\widehat{\mathbf1_{\mathcal O_F}}=\mathbf1_{\mathcal O_F}.
$$

For the canonical character induced from $\mathbb Q_p$, the annihilator is instead the [inverse different](../../../../../inverse-different.md) and the displayed general formula applies.

If $g(x)=f(ax+b)$ with $a\ne0$, the substitution $u=ax+b$ and the scaling rule $dx=|a|^{-1}du$ give

$$
\begin{aligned}
\widehat g(y)
&=\int_Ff(ax+b)\psi(xy)\,dx\\
&=|a|^{-1}\int_Ff(u)\psi((u-b)y/a)\,du\\
&=\psi(-by/a)|a|^{-1}\widehat f(y/a).
\end{aligned}
$$

Every locally constant compactly supported function is a finite linear combination of characteristic functions of cosets $b+a\mathcal O_F$: compactness extracts finitely many cosets on which the function is constant. The formula just proved, together with the transform of $\mathbf1_{\mathcal O_F}$, shows that the transform of each such characteristic function is again locally constant and compactly supported. Therefore the [Fourier transform over a local field](../../../../../fourier-transform-over-a-local-field.md) maps $\mathcal S(F)$ to itself.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 123](../../paper-123-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
