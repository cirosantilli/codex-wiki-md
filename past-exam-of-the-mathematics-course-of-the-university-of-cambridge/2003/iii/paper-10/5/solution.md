<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $C$ be a [cotype 2](../../../../../cotype-2.md) constant of $Y$. All [bounded linear operators](../../../../../continuous-linear-operator.md) from $\ell_\infty^N$ have finite p-summing norms: writing $Tx=\sum_{k=1}^Nx_ky_k$ and using the [triangle inequality](../../../../../triangle-inequality.md) in the finite-family $\ell^p$ norm gives $\pi_p(T)\le\sum_k\|y_k\|$. Thus applying the [Pietsch factorization theorem](../../../../../pietsch-factorization-theorem.md) below is legitimate.

First let $a_4=\pi_4(T)$, and use the [Pietsch factorization theorem](../../../../../pietsch-factorization-theorem.md) to choose a [probability measure](../../../../../probability-measure.md) $\mu$ on the dual unit ball $B_{\ell_1^N}$. For a finite family $x_j\in\ell_\infty^N$, the [cotype 2](../../../../../cotype-2.md) inequality and [Pietsch factorization theorem](../../../../../pietsch-factorization-theorem.md) domination give

$$
\left(\sum_j\|Tx_j\|^2\right)^{1/2}
\le C\left(\mathbb E\left\|T\sum_j\varepsilon_jx_j\right\|^2\right)^{1/2}
\le Ca_4\left[\mathbb E\left(\int\left|\sum_j\varepsilon_j\phi(x_j)\right|^4d\mu(\phi)\right)^{1/2}\right]^{1/2}.
$$

The [Jensen inequality](../../../../../jensen-s-inequality.md) bounds the final bracket by $[\int\mathbb E|\sum_j\varepsilon_j\phi(x_j)|^4d\mu]^{1/4}$. For real or complex scalars,

$$
\mathbb E\left|\sum_j\varepsilon_jb_j\right|^4\le3\left(\sum_j|b_j|^2\right)^2.
$$

For complex scalars, paired-index expansion gives $\mathbb E|\sum_j\varepsilon_jb_j|^4=2(\sum_j|b_j|^2)^2+|\sum_jb_j^2|^2-2\sum_j|b_j|^4$, which is at most the displayed bound by the [triangle inequality](../../../../../triangle-inequality.md). For real scalars this reduces to $3(\sum b_j^2)^2-2\sum b_j^4$. Since $\mu$ is a [probability measure](../../../../../probability-measure.md) on the dual unit ball, we obtain

$$
\left(\sum_j\|Tx_j\|^2\right)^{1/2}\le3^{1/4}Ca_4\sup_{\phi\in B_{\ell_1^N}}\left(\sum_j|\phi(x_j)|^2\right)^{1/2}.
$$

Taking the least constant proves **$\pi_2(T)\le K\pi_4(T)$ with $K=3^{1/4}C$**, uniformly in $N$.

We next prove a summing-norm interpolation estimate using coordinate truncation. Put $a=\pi_2(T)$ and $M=\|T\|$, assuming $T\ne0$. The [Pietsch factorization theorem](../../../../../pietsch-factorization-theorem.md) for $p=2$ gives a measure $\mu$ on $B_{\ell_1^N}$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
|\phi(x)|^2\le\left(\sum_i|\phi_i|\right)\sum_i|\phi_i||x_i|^2\le\sum_i|\phi_i||x_i|^2.
$$

Set $\nu_i=\int|\phi_i|\,d\mu$. Their sum is at most one; adding the missing mass to one coordinate, if necessary, makes $(\nu_i)$ a probability vector and preserves domination. Hence

$$
\|Tx\|\le a\left(\sum_i\nu_i|x_i|^2\right)^{1/2}.
$$

Write $r=(\sum_i\nu_i|x_i|^4)^{1/4}$. For $t>0$, clip each coordinate of $x$ at magnitude $t$, obtaining $z_i=x_i\min(1,t/|x_i|)$, with $z_i=0$ if $x_i=0$. Set $w=x-z$. Then $\|z\|_\infty\le t$ and

$$
\sum_i\nu_i|w_i|^2\le\sum_{|x_i|>t}\nu_i|x_i|^2\le t^{-2}\sum_i\nu_i|x_i|^4=r^4/t^2.
$$

The [triangle inequality](../../../../../triangle-inequality.md) and the two different bounds on $T$ now give $\|Tx\|\le Mt+ar^2/t$. For $r>0$, take $t=r\sqrt{a/M}$; if $r=0$, domination already gives $Tx=0$. Consequently

$$
\|Tx\|\le2\sqrt{Ma}\left(\sum_i\nu_i|x_i|^4\right)^{1/4}.
$$

Summing fourth powers over any family $(x_j)$ gives

$$
\sum_j\|Tx_j\|^4\le16M^2a^2\sum_i\nu_i\sum_j|(x_j)_i|^4\le16M^2a^2 w_4(x_1,\ldots,x_m)^4,
$$

since each coordinate evaluation belongs to the dual unit ball. Therefore $\pi_4(T)\le2\sqrt{M\pi_2(T)}$. Combine this with the first estimate:

$$
a\le2K\sqrt{Ma}\quad\Longrightarrow\quad
\boxed{\pi_2(T)\le L\|T\|,\qquad L=4K^2=4\sqrt3\,C^2.}
$$

The zero operator also satisfies this inequality. Both constants depend only on $Y$, through its [cotype 2](../../../../../cotype-2.md) constant, and not on $N$.

Finally let $E\subset Y$ have dimension $N$, with its inherited [norm](../../../../../norm.md). The permitted finite-dimensional identity result is $\pi_2(I_E)=\sqrt N$. The inclusion $J:E\to Y$ is an [isometric embedding](../../../../../isometric-embedding.md), so $\pi_2(J)=\pi_2(I_E)$. For every [Banach space isomorphism](../../../../../banach-space-isomorphism.md) $S:\ell_\infty^N\to E$, apply the preceding estimate to $T=JS$ and the ideal property of [absolutely p-summing operators](../../../../../absolutely-p-summing-operator.md):

$$
\sqrt N=\pi_2(J)=\pi_2(TS^{-1})\le\pi_2(T)\|S^{-1}\|\le L\|S\|\|S^{-1}\|.
$$

The [Banach-Mazur distance](../../../../../banach-mazur-distance.md) is the infimum of this last product over $S$, and therefore

$$
\boxed{d(E,\ell_\infty^N)\ge L^{-1}\sqrt N.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
