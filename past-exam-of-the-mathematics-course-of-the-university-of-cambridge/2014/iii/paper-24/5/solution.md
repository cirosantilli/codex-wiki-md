<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For this non-Archimedean [local field](../../../../../local-field.md), the [Schwartz-Bruhat space](../../../../../schwartz-bruhat-space.md) $\mathcal S(F)$ consists of locally constant, compactly supported complex-valued functions. Choose a nontrivial continuous [additive character](../../../../../additive-character.md) $\psi:F\to\mathbb C^\times$ of modulus one and an additive [Haar measure](../../../../../haar-measure.md) $dx$. We use the plus-sign convention for the [Fourier transform over a local field](../../../../../fourier-transform-over-a-local-field.md):

$$
\widehat f(y)=\int_F f(x)\psi(xy)\,dx.
$$

Compact support makes the integral absolutely convergent. The [additive character](../../../../../additive-character.md) and the scale of the [Haar measure](../../../../../haar-measure.md) are part of the definition; without them there is no canonical numerical transform.

Let $q=|\mathcal O_F/\pi_F\mathcal O_F|$, and write $V=\operatorname{vol}(\mathcal O_F)$. Define the integer $c$ by the [annihilator of the valuation ring](../../../../../annihilator-of-the-valuation-ring.md) $\mathcal O_F^\perp=\pi_F^c\mathcal O_F$. Equivalently, $\psi$ is trivial on $\pi_F^c\mathcal O_F$ and not on $\pi_F^{c-1}\mathcal O_F$. Such a conductor exists: continuity puts the image of some additive ball inside an arc containing no nontrivial circle subgroup, so the character is trivial on that ball; nontriviality bounds the possible ball exponents below. Then $H_n=\pi_F^n\mathcal O_F$ has volume $Vq^{-n}$ and [character annihilator](../../../../../character-annihilator.md) $H_n^\perp=\pi_F^{c-n}\mathcal O_F$.

Translation gives

$$
\widehat{\mathbf1_{a+H_n}}(y)=\psi(ay)\int_{H_n}\psi(ty)\,dt.
$$

The integral is the volume if $y\in H_n^\perp$. Otherwise translate it by $t_0\in H_n$ with $\psi(t_0y)\ne1$; [Haar measure](../../../../../haar-measure.md) invariance multiplies the same integral by a nonidentity scalar, so it must vanish. Thus

$$
\boxed{\widehat{\mathbf1_{a+\pi_F^n\mathcal O_F}}(y)=Vq^{-n}\psi(ay)\mathbf1_{\pi_F^{c-n}\mathcal O_F}(y).}
$$

Every [Schwartz-Bruhat function](../../../../../schwartz-bruhat-function.md) is a finite linear combination of such coset indicators: compactness of its support supplies a common sufficiently small translation subgroup on which it is constant, and finitely many of its cosets cover the support. The transform of each indicator has compact support and is locally constant, since $\psi$ has open kernel. Consequently **$\widehat f\in\mathcal S(F)$ for every $f\in\mathcal S(F)$**.

Apply the transform again to an indicator. The same character-orthogonality calculation, together with $(H_n^\perp)^\perp=H_n$, gives

$$
\widehat{\widehat{\mathbf1_{a+H_n}}}(x)=Vq^{-n}\operatorname{vol}(H_n^\perp)\mathbf1_{H_n}(-x-a)=V^2q^{-c}\mathbf1_{a+H_n}(-x).
$$

Choose the [self-dual Haar measure](../../../../../self-dual-haar-measure.md), characterized here by $V=q^{c/2}$. By linearity the desired [Fourier inversion](../../../../../fourier-inversion-theorem.md) is

$$
\boxed{\widehat{\widehat f}(x)=f(-x).}
$$

In particular, one may rescale any nontrivial [additive character](../../../../../additive-character.md) to make $c=0$, and then take $V=1$. For a concrete construction, start with $\psi_0(x)=\psi_{\mathbb Q_p}(\operatorname{Tr}_{F/\mathbb Q_p}x)$, where the standard rational [additive character](../../../../../additive-character.md) has kernel $\mathbb Z_p$. Its annihilator is the [inverse different](../../../../../inverse-different.md) $\mathfrak D_{F/\mathbb Q_p}^{-1}$. If that ideal is $\pi_F^{-d}\mathcal O_F$, the rescaled character $\psi(x)=\psi_0(\pi_F^{-d}x)$ has $\mathcal O_F^\perp=\mathcal O_F$. This supplies the stated normalization and also explains how the [different ideal](../../../../../different-ideal.md) enters local [Fourier analysis](../../../../../fourier-analysis-split.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
