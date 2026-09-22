<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

There is a normalization omission in the printed conclusion: the discrepancy of a count of pairs must be bounded by a small function of the energy excess times $N^2$. We prove this normalized result, then give a counterexample to the literal bound without $N^2$. Write $\epsilon$ for the energy excess parameter to avoid confusing it with an element of the third set.

For [Fourier analysis on a finite abelian group](../../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md), use $e_N(t)=e^{2\pi it/N}$ and

$$
\widehat h(r)=\mathbb E_{x\in\mathbb Z_N}h(x)e_N(-rx).
$$

Character orthogonality, $\mathbb E_x e_N(rx)=1$ for $r=0$ and zero otherwise, gives [Fourier inversion](../../../../../../fourier-inversion-theorem.md) and the [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md):

$$
h(x)=\sum_r\widehat h(r)e_N(rx),\qquad \sum_r|\widehat h(r)|^2=\mathbb E_x|h(x)|^2.
$$

Put $u=1_A$, $v=1_B$, $w=1_C$. Expanding the constraint $a_1+a_2=a_3+a_4$ by the same character orthogonality gives the [additive energy](../../../../../../additive-energy.md) identity

$$
\frac{E(A)}{N^3}=\sum_r|\widehat u(r)|^4=\alpha^4+\sum_{r\ne0}|\widehat u(r)|^4.
$$

Thus $\sum_{r\ne0}|\widehat u(r)|^4\leq\epsilon$, and every nonconstant [Fourier coefficient on a finite abelian group](../../../../../../fourier-coefficient-on-a-finite-abelian-group.md) of $u$ has modulus at most $\epsilon^{1/4}$. Expanding the constraint in the triple count $T$ gives

$$
\frac{T}{N^2}=\sum_r\widehat u(r)\widehat w(r)\widehat v(-2r)=\alpha\beta\gamma+\sum_{r\ne0}\widehat u(r)\widehat w(r)\widehat v(-2r).
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) yields

$$
\left|\frac{T}{N^2}-\alpha\beta\gamma\right|\leq\epsilon^{1/4}\left(\sum_r|\widehat w(r)|^2\right)^{1/2}\left(\sum_r|\widehat v(-2r)|^2\right)^{1/2}.
$$

The first squared norm is $\gamma$ by the [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md). For the second, multiplication by $2$ on $\mathbb Z_N$ has kernel size $h=\gcd(2,N)$ and every element of its image has exactly $h$ preimages. Hence

$$
\sum_r|\widehat v(-2r)|^2=h\sum_{s\in2\mathbb Z_N}|\widehat v(s)|^2\leq h\beta.
$$

This proves that [additive energy controls three-term progression mixing](../../../../../../additive-energy-controls-three-term-progression-mixing.md), including for even moduli:

$$
\boxed{|T-\alpha\beta\gamma N^2|\leq\sqrt{\gcd(2,N)\beta\gamma}\,\epsilon^{1/4}N^2\leq\sqrt2\,\epsilon^{1/4}N^2.}
$$

Thus the intended density-error function can be $F(\epsilon)=\sqrt2\,\epsilon^{1/4}$, which tends to zero. For odd moduli the factor $\sqrt2$ can be replaced by one.

To see why the literal unnormalized conclusion is false, take $N=q^2$ and let all three sets be the subgroup of multiples of $q$. Their densities are $1/q$. Every choice of three entries of that subgroup determines the fourth entry of an additive quadruple, so its energy is $q^3$. The excess parameter is

$$
\epsilon=\frac1{q^3}-\frac1{q^4}=\frac{q-1}{q^4}\longrightarrow0.
$$

Every pair $(a,b)$ in the subgroup determines $c=2b-a$ there, giving $T=q^2$, whereas $\alpha\beta\gamma N^2=q$. Their difference is $q^2-q\to\infty$, which cannot be bounded by any function of $\epsilon$ tending to zero. The missing $N^2$ is therefore a genuine source defect, not an alternative [Fourier transform](../../../../../../fourier-transform.md) normalization.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
