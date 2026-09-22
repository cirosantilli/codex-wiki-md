<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take a nonzero eigenform of positive weight, and put $h(\tau)=f(p\tau)$ and $C=\chi(p)p^{k-1}$. The original form belongs to level $Np$ by inclusion of groups. For $\gamma=\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\Gamma_0(Np)$, the conjugate $\begin{pmatrix}a&pb\\c/p&d\end{pmatrix}$ lies in $\Gamma_0(N)$, so

$$
h(\gamma\tau)=\chi(d)(c\tau+d)^kh(\tau).
$$

Its [Dirichlet character](../../../../../../dirichlet-character.md) is therefore the specified reduced [Dirichlet character](../../../../../../dirichlet-character.md); [modular cusp](../../../../../../cusp-of-a-modular-group.md) holomorphy is permitted in the question. This is the [Dirichlet character](../../../../../../dirichlet-character.md) version of an [oldform by argument dilation](../../../../../../oldform-by-argument-dilation.md).

A nonzero positive-weight [modular form](../../../../../../modular-form.md) cannot be constant, because the [matrix](../../../../../../matrix.md) $\begin{pmatrix}1&0\\N&1\end{pmatrix}$ would force a nonzero constant to equal $(N\tau+1)^k$ times itself. Let $n_0>0$ be its first nonzero positive Fourier index. In a relation $Af+Bh=0$, the $q^{n_0}$ coefficient forces $A=0$, then $B=0$. Hence their span is two-dimensional, even when the original constant term is nonzero.

At the new level $p$ is a bad prime, so its operator is $U_p$. The good-prime eigenrelation at the old level and part (c) give

$$
U_pf=\lambda f-Ch,\qquad U_ph=f.
$$

Thus the [matrix](../../../../../../matrix.md) in the ordered basis $(f,h)$ is

$$
\boxed{\begin{pmatrix}\lambda&1\\-C&0\end{pmatrix},}
$$

with [characteristic polynomial](../../../../../../characteristic-polynomial.md) $X^2-\lambda X+C$. For its distinct roots,

$$
\boxed{f-\beta f(p\tau)\text{ has eigenvalue }\alpha,\qquad f-\alpha f(p\tau)\text{ has eigenvalue }\beta.}
$$

This is [prime stabilization of an oldform](../../../../../../prime-stabilization-of-an-oldform.md).

The nonzero positive-weight qualification is necessary for the two-dimensional assertion. The zero form gives no such span, and if weight zero is allowed, $f=1$ at trivial [Dirichlet character](../../../../../../dirichlet-character.md) has distinct good-prime roots $1$ and $p^{-1}$, while $f(\tau)=f(p\tau)$ spans only one dimension. The asserted result uses the usual nonzero positive-weight eigenform setting.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
