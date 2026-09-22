<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose compatible primitive [roots of unity](../../../../../../root-of-unity.md) $\zeta_{p^{n+1}}$, with $\zeta_{p^{n+2}}^p=\zeta_{p^{n+1}}$. Use the slightly faster-converging series permitted by “or otherwise”:

$$
A_N=\sum_{n=0}^Np^{2n}\zeta_{p^{n+1}}.
$$

The terms have [field absolute value](../../../../../../absolute-value-algebra.md) $p^{-2n}$, so the partial sums are a [Cauchy sequence](../../../../../../cauchy-sequence.md) in $\overline{\mathbb Q}_p$. We show that an algebraic limit would contradict the growth of cyclotomic extension degrees. The faster weights make the strict conjugate-distance estimate work uniformly also at $p=2$.

Put $L_N=\mathbb Q_p(\zeta_{p^{N+1}})$. Its degree is $p^N(p-1)$: the translated [cyclotomic polynomial](../../../../../../cyclotomic-polynomial.md) $\Phi_{p^{N+1}}(1+T)$ has constant term $p$ and reduces modulo $p$ to $T^{p^N(p-1)}$, so is Eisenstein. To verify the reduction, write it as $\sum_{j=0}^{p-1}(1+T)^{jp^N}$ and use characteristic $p$ to reduce this to $\sum_{j=0}^{p-1}(1+T^{p^N})^j=T^{p^N(p-1)}$. All roots lie in $L_N$, and its Galois automorphisms are $\sigma_a(\zeta)=\zeta^a$ for units $a$ modulo $p^{N+1}$.

For a nonidentity automorphism, put $r=v_p(a-1)$, choosing a representative with $0\le r\le N$. It fixes the terms with $n<r$. For $n\ge r$, the root $\zeta_{p^{n+1}}^{a-1}$ has order $p^{n+1-r}$, so the root-of-unity [valuation](../../../../../../valuation.md) formula, with $v_p(p)=1$, gives

$$
v_p\!\left(p^{2n}(\sigma_a\zeta_{p^{n+1}}-\zeta_{p^{n+1}})\right)=2n+\frac1{p^{n-r}(p-1)}.
$$

This is strictly increasing as $n$ increases: successive differences are $2-p^{-(n-r+1)}>0$. Thus the first changed term is the unique term of smallest [valuation](../../../../../../valuation.md) and cannot cancel. Consequently

$$
v_p(\sigma_aA_N-A_N)=2r+\frac1{p-1}\le2N+\frac1{p-1}.
$$

In particular no nonidentity automorphism fixes $A_N$, so $\mathbb Q_p(A_N)=L_N$. Also the distance from $A_N$ to every distinct conjugate is at least $p^{-2N-1/(p-1)}$.

Suppose the [Cauchy sequence](../../../../../../cauchy-sequence.md) converged to $A\in\overline{\mathbb Q}_p$. The tail estimate gives

$$
|A-A_N|_p\le p^{-2N-2}<p^{-2N-1/(p-1)}.
$$

Apply [Krasner's lemma](../../../../../../krasner-s-lemma.md) with $\alpha=A_N$, $\beta=A$. It forces $L_N=\mathbb Q_p(A_N)\subseteq\mathbb Q_p(A)$ for every $N$. The right-hand side has finite degree, while $[L_N:\mathbb Q_p]=p^N(p-1)$ is unbounded, a contradiction. Therefore

$$
\boxed{\overline{\mathbb Q}_p\text{ is not complete}.}
$$

This proves [algebraic closure of the p-adic numbers is not complete](../../../../../../algebraic-closure-of-the-p-adic-numbers-is-not-complete.md) by an explicit algebraic [Cauchy sequence](../../../../../../cauchy-sequence.md) and a fully quantified conjugate-separation argument.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
