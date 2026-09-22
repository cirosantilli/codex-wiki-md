<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Separate the constant embedding coordinate from its nonzero modes. Its integral gives the momentum-conservation delta function; below this is understood and absorbed into the amplitude normalization on the momentum-conserving locus. For the nonzero modes the Euclidean [Polyakov action](../../../../../polyakov-action.md) is quadratic, with [worldsheet Green function](../../../../../worldsheet-green-function.md)

$$
\langle X^\mu(z)X^\nu(w)\rangle=-\frac{\alpha'}2\eta^{\mu\nu}\log|z-w|^2.
$$

Treat the [tachyon](../../../../../tachyon.md) vertex operators as normal ordered, removing coincident self-contractions. The [Gaussian functional integral](../../../../../gaussian-functional-integral.md), or the same calculation by [Wick's theorem](../../../../../wick-s-theorem.md), gives

$$
\left\langle\prod_r:e^{ik_r\cdot X(z_r)}:\right\rangle=\exp\left(-\sum_{r<s}k_r\cdot k_s\langle X(z_r)X(z_s)\rangle\right)=\prod_{r<s}|z_r-z_s|^{\alpha' k_r\cdot k_s}.
$$

All remaining determinants are independent of the insertion points and [momenta](../../../../../momentum.md) and enter the overall constant. This derives the [Koba-Nielsen factor](../../../../../koba-nielsen-factor.md) and the requested position integral.

For the [Möbius transformation](../../../../../mobius-transformation.md) $f(z)=(az+b)/(cz+d)$, $ad-bc=1$, one has

$$
f(z_r)-f(z_s)=\frac{z_r-z_s}{(cz_r+d)(cz_s+d)},\qquad d^2f(z_r)=|cz_r+d|^{-4}d^2z_r.
$$

The transformed [Koba-Nielsen factor](../../../../../koba-nielsen-factor.md) contributes, at insertion $r$, the power $-\alpha'\sum_{s\ne r}k_r\cdot k_s$ of $|cz_r+d|$. [Four-momentum conservation](../../../../../four-momentum-conservation.md) makes this power $\alpha'k_r^2$. The complete differential integrand therefore transforms by

$$
\prod_r|cz_r+d|^{\alpha'k_r^2-4}.
$$

It is **invariant when $\alpha'k_r^2=4$ for every external [tachyon](../../../../../tachyon.md)**. The correlator alone is covariant; the integration measures are necessary for invariance. The [group](../../../../../group-split.md) acting faithfully on the sphere is $PSL(2,\mathbb C)$, with the two elements $\pm I$ of $SL(2,\mathbb C)$ acting identically.

The apparent integral over all positions includes the residual conformal-group gauge volume. Divide by it and fix three distinct insertions. The [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md), equivalently the [three-point worldsheet ghost correlator](../../../../../three-point-worldsheet-ghost-correlator.md) and its conjugate, contributes

$$
J=|(z_1-z_2)(z_2-z_4)(z_4-z_1)|^2.
$$

Set $z_1=\Lambda$, $z_2=0$, $z_4=1$, then send $\Lambda$ to infinity on the sphere; the sign of the real direction is irrelevant. The factors involving $z_1$ behave as $|\Lambda|^{\alpha' k_1\cdot\sum_{s\ne1}k_s}=|\Lambda|^{-4}$, while $J\sim|\Lambda|^4$. They cancel, leaving $z_3=z$ as the one integration variable.

The remaining distance exponents are

$$
\alpha'k_2\cdot k_3=-4-\frac{\alpha't}{2},\qquad \alpha'k_3\cdot k_4=-4-\frac{\alpha's}{2}.
$$

For example $(k_2+k_3)^2=(k_1+k_4)^2=-t$ and each individual squared [momentum](../../../../../momentum.md) is $4/\alpha'$. Also

$$
s+t+u=-\sum_{r=1}^4k_r^2=-\frac{16}{\alpha'}.
$$

Consequently the reduced amplitude is proportional to

$$
\int_{\mathbb C}d^2z\,|z|^{-4-\alpha't/2}|1-z|^{-4-\alpha's/2}.
$$

Apply the supplied complex beta integral with $A=4+\alpha't/2$, $B=4+\alpha's/2$, and $C=4-A-B=4+\alpha'u/2$. Its numerator arguments become $-1-\alpha't/4$, $-1-\alpha's/4$, $-1-\alpha'u/4$, while its denominator arguments become $2+\alpha'u/4$, $2+\alpha't/4$, $2+\alpha's/4$. Thus **the four-point amplitude is the [Virasoro–Shapiro amplitude](../../../../../virasoro-shapiro-amplitude.md)**

$$
\boxed{T_4=C_0\frac{\Gamma(-1-\alpha's/4)\Gamma(-1-\alpha't/4)\Gamma(-1-\alpha'u/4)}{\Gamma(2+\alpha's/4)\Gamma(2+\alpha't/4)\Gamma(2+\alpha'u/4)},}
$$

where $C_0$ is momentum-independent. The integral converges initially when $\operatorname{Re}A<2$, $\operatorname{Re}B<2$, and $\operatorname{Re}(A+B)>2$; the displayed answer elsewhere is its [analytic continuation](../../../../../analytic-continuation.md).

The [gamma function](../../../../../gamma-function.md) has [simple poles](../../../../../simple-pole.md) at nonpositive integers and no zeros. At generic fixed $t$, the amplitude therefore has **simple $s$-channel poles at $s=4(n-1)/\alpha'$, $n=0,1,2,\ldots$**, with the same towers in $t$ and $u$ by [crossing symmetry](../../../../../crossing-symmetry.md). They describe exchange of the [closed string](../../../../../closed-string.md) [tachyon](../../../../../tachyon.md), massless states, and the infinitely many massive levels. The reciprocal denominator factors can give zeros at negative values $s=-4(\ell+2)/\alpha'$; special kinematics can also make an exchange [residue](../../../../../residue.md) vanish.

To see the structure of a generic [residue](../../../../../residue.md), set $a=-1-\alpha's/4$, $b=-1-\alpha't/4$, $c=-1-\alpha'u/4$, so $a+b+c=1$. At $a=-n$, the [Gamma function recurrence](../../../../../gamma-function-recurrence.md) reduces the remaining factors to a constant times $\prod_{j=1}^n(b-j)^2$. The [Virasoro–Shapiro amplitude pole residue](../../../../../virasoro-shapiro-amplitude-pole-residue.md) is thus a polynomial of degree $2n$ in the other channel invariant, consistent with exchange up to spin $2n$. Crossed numerator poles must not simply be multiplied: near $a=-n+\delta$ and $b=-m+\varepsilon$, $c=1+n+m-\delta-\varepsilon$, and the zero of $1/\Gamma(1-c)$ cancels the putative double pole. The leading singular part is proportional to

$$
\binom{n+m}{n}^{\!2}\left(\frac1\delta+\frac1\varepsilon\right).
$$

The tree amplitude is [meromorphic](../../../../../meromorphic-function.md), with no loop threshold branch cuts; its channel singularities express factorization and string dual resonance.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
