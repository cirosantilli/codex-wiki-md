<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define the normalized progression average

$$
\Lambda_4(f_0,f_1,f_2,f_3)=\mathbb E_{x,d}\prod_{j=0}^3f_j(x+jd).
$$

We first prove the needed [four-term progression bound with torsion factors](../../../../../../four-term-progression-bound-with-torsion-factors.md), valid for the arbitrary cyclic modulus in the question:

$$
|\Lambda_4(f_0,f_1,f_2,f_3)|\le6^{1/8}\min_j\|f_j\|_{U^3}\qquad(|f_j|\le1).
$$

For the factor at slope zero, write $y=x+3d$, $t=d$, and apply [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) to discard $f_3(y)$:

$$
|\Lambda_4|^2\le\mathbb E_y\left|\mathbb E_t f_0(y-3t)f_1(y-2t)f_2(y-t)\right|^2.
$$

For concise bookkeeping put $D_hf(x)=f(x)\overline{f(x+h)}$, the conjugate of the preceding derivative convention, and $F_{i,h}=D_{-(3-i)h}f_i$. Expanding the square with $t,t+h$ and setting $z=y-t$ gives $\mathbb E_{z,t,h}F_{0,h}(z-2t)F_{1,h}(z-t)F_{2,h}(z)$. Another [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md), now in $(z,h)$, discards $F_{2,h}$ and yields

$$
|\Lambda_4|^4\le\mathbb E_{z,h}\left|\mathbb E_tF_{0,h}(z-2t)F_{1,h}(z-t)\right|^2.
$$

Expand with $t,t+k$, set $w=z-t$, and apply [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) a third time to discard $D_{-k}F_{1,h}(w)$. The remaining $t$-average is a full average over $x=w-t$, so

$$
|\Lambda_4|^8\le\mathbb E_{h,k}\left|\mathbb E_xD_{-2k}D_{-3h}f_0(x)\right|^2.
$$

Negating $h,k$ does not change the average. The nonnegative integrand depends only on $2k$ and $3h$. Averaging over the subgroups $2\mathbb Z_N$ and $3\mathbb Z_N$ costs at most their indices $t_2=\gcd(2,N)$ and $t_3=\gcd(3,N)$ compared with unrestricted increments. The unrestricted expression is exactly $\|f_0\|_{U^3}^8$, obtained by expanding the last squared average. Thus the bound is $(t_2t_3)^{1/8}\|f_0\|_{U^3}\le6^{1/8}\|f_0\|_{U^3}$.

Reversing the progression handles slope three. To isolate slope one, eliminate slopes three, zero and two successively in the same calculation; the surviving increments have coefficients $-2,1,-1$, so only the index $t_2$ is needed. Reversal handles slope two. This proves the minimum-over-factors bound, without assuming that $2$ or $3$ is invertible modulo $N$.

If $\delta=0$, the requested lower bound is zero and is immediate. Otherwise let $g=1_A-\delta$. Telescoping the product of four copies of $1_A=\delta+g$ against the constant product $\delta^4$ gives four error terms, each with one factor $g$ and three factors bounded by one. Hence

$$
|\Lambda_4(1_A,1_A,1_A,1_A)-\delta^4|\le4\cdot6^{1/8}\|g\|_{U^3}
\le4\cdot6^{1/8}\alpha^{1/8}.
$$

In particular, choosing $\alpha\le\delta^{32}/(6\cdot8^8)$ gives

$$
\boxed{\#\{(x,d):x,x+d,x+2d,x+3d\in A\}\ge\frac12\delta^4N^2.}
$$

These are ordered modular progression parameters $(x,d)$, as requested; small-order differences and $d=0$ are included. A claim of distinct nontrivial progressions would need a separate subtraction and size condition.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
