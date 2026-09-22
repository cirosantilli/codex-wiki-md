<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\Gamma=SL_2(\mathbb Z)$ and $G=GL_2(\mathbb Q)^+$. The [double-coset Hecke algebra](../../../../../../double-coset-hecke-algebra.md) consists of $\Gamma$-bi-invariant complex [functions](../../../../../../function-split.md) on $G$ supported on finitely many [double cosets](../../../../../../double-coset.md), with convolution

$$
(h_1*h_2)(g)=\sum_{\Gamma x\in\Gamma\backslash G}h_1(gx^{-1})h_2(x).
$$

Each [double coset](../../../../../../double-coset.md) has finitely many orbits under left multiplication by $\Gamma$, by [rational conjugation of finite-index modular subgroups](../../../../../../rational-conjugation-of-finite-index-modular-subgroups.md). Thus the sum is finite and independent of representatives. The characteristic functions of the [double cosets](../../../../../../double-coset.md) form its basis, and its right action on invariant [modular forms](../../../../../../modular-form.md) is $f*h=\sum_{\Gamma x}h(x)f|_kx$, using the [determinant-normalized slash operator](../../../../../../determinant-normalized-slash-operator.md).

For a positive integer $n$, let $\mathcal M_n$ be all integral two-by-two [matrices](../../../../../../matrix.md) of positive [determinant](../../../../../../determinant.md) $n$. It is $\Gamma$-bi-invariant. Define $T(n)$ to be its [indicator function](../../../../../../indicator-function.md), equivalently the sum of the distinct [double cosets](../../../../../../double-coset.md) it contains, each with coefficient one. This is the convention consistent with the requested formula. For composite $n$, it need not be the single [double coset](../../../../../../double-coset.md) of $\operatorname{diag}(1,n)$: for instance $2I\in\mathcal M_4$ cannot lie in that [double coset](../../../../../../double-coset.md), since multiplying by unimodular integral [matrices](../../../../../../matrix.md) preserves the greatest common divisor of the entries.

Prove all the needed subgroup facts directly. For a [finite-index subgroup](../../../../../../finite-index-subgroup.md) $L\subseteq\mathbb Z^2$, take $a$ to be the least positive first coordinate appearing in $L$ and $d$ the least positive second coordinate on its intersection with the second axis. Euclidean division then shows that the first-coordinate projection is $a\mathbb Z$ and $L\cap(\{0\}\times\mathbb Z)=\{0\}\times d\mathbb Z$. Positivity follows, for example, because the finite [quotient group](../../../../../../quotient-group.md) kills a nonzero multiple of each coordinate vector. Choose $(a,b)\in L$ and reduce $b$ modulo $d$ to $0\leq b<d$. Every vector of $L$ has first coordinate a multiple of $a$, and subtracting that multiple of $(a,b)$ leaves a multiple of $(0,d)$. Therefore these two vectors form a [basis](../../../../../../basis.md) of $L$. The parameters $a,d,b$ are unique. Reducing the first coordinate modulo $a$ and then the second modulo $d$ gives precisely $ad$ quotient representatives, so $[\mathbb Z^2:L]=ad$.

Apply this [row Hermite normal form in rank two](../../../../../../row-hermite-normal-form-in-rank-two.md) to the [row lattice](../../../../../../row-lattice-of-an-integer-matrix.md) of an integral [matrix](../../../../../../matrix.md) $A$ with $\det A=n$. Its [row lattice](../../../../../../row-lattice-of-an-integer-matrix.md) contains $n\mathbb Z^2$, since $\operatorname{adj}(A)A=nI$, so it has finite index. Its two rows and the displayed two rows are [bases](../../../../../../basis.md) of the same [row lattice](../../../../../../row-lattice-of-an-integer-matrix.md). The two inverse change-of-basis [matrices](../../../../../../matrix.md) have integer entries, so their [determinants](../../../../../../determinant.md) are integers whose product is one. Thus the change-of-basis [matrix](../../../../../../matrix.md) has [determinant](../../../../../../determinant.md) $\pm1$; since both orientations are positive, its [determinant](../../../../../../determinant.md) is one. Thus each orbit under left multiplication by $\Gamma$ has exactly one of the [determinant-n matrix representatives for Hecke operators](../../../../../../determinant-n-matrix-representatives-for-hecke-operators.md)

$$
\begin{pmatrix}a&b\\0&d\end{pmatrix},\qquad a,d>0,\quad ad=n,\quad0\leq b<d.
$$

There are $\sum_{d\mid n}d$ such representatives, proving finiteness as well as the formula. The subgroup argument is a proof of the relevant [Hermite normal form](../../../../../../hermite-normal-form.md), not an invocation of an unproved lattice classification.

Consequently the normalized [Hecke operator](../../../../../../hecke-operator.md) is

$$
\boxed{T_nf=n^{k/2-1}\sum_{ad=n}\sum_{b=0}^{d-1}
 f|_k\begin{pmatrix}a&b\\0&d\end{pmatrix}.}
$$

It preserves $M_k(\Gamma)$: right multiplication by $\Gamma$ permutes the left-multiplication orbits in $\mathcal M_n$, giving invariance, and [cusp holomorphy under rational slash operators](../../../../../../cusp-holomorphy-under-rational-slash-operators.md) gives the holomorphy of each term at every cusp.

For a triangular representative the [determinant-normalized slash operator](../../../../../../determinant-normalized-slash-operator.md) is $f|_kA=n^{k/2}d^{-k}f((az+b)/d)$. Summing the [Fourier expansion of a modular form](../../../../../../fourier-expansion-of-a-modular-form.md) over $b$ kills every index not divisible by $d$, by finite exponential orthogonality. Thus

$$
T_nf=n^{k-1}\sum_{ad=n}d^{1-k}\sum_{\ell\geq0}a_{d\ell}(f)q^{a\ell}.
$$

The [Fourier coefficients of a composite-index Hecke operator](../../../../../../fourier-coefficients-of-a-composite-index-hecke-operator.md) are therefore

$$
\boxed{a_r(T_nf)=\sum_{a\mid\gcd(n,r)}a^{k-1}a_{nr/a^2}(f)\quad(r\geq1),
\qquad a_0(T_nf)=\sigma_{k-1}(n)a_0(f).}
$$

In particular $a_1(T_nf)=a_n(f)$. If $T_nf=\lambda f$, comparison of the $q$ coefficients gives

$$
\boxed{a_n(f)=\lambda a_1(f).}
$$

Finally suppose $a_0(f)\ne0$ and $f$ is a simultaneous eigenfunction. Constant coefficients force $\lambda_n=\sigma_{k-1}(n)$, so $a_n(f)=a_1(f)\sigma_{k-1}(n)$ for all $n\geq1$. Weight two cannot occur, by [vanishing of weight-two level-one modular forms](../../../../../../vanishing-of-weight-two-level-one-modular-forms.md). For even $k\geq4$, use the normalized [Eisenstein series](../../../../../../eisenstein-series.md) with its [Fourier expansion of a normalized Eisenstein series](../../../../../../fourier-expansion-of-a-normalized-eisenstein-series.md)

$$
E_k=1+c_k\sum_{n\geq1}\sigma_{k-1}(n)q^n,
\qquad c_k=-\frac{2k}{B_k}\ne0,
$$

where $B_k$ is the [Bernoulli number](../../../../../../bernoulli-number.md). Then $h=f-a_0(f)E_k$ is a [cusp form](../../../../../../cusp-form.md) with coefficients $(a_1(f)-a_0(f)c_k)\sigma_{k-1}(n)$. The [Fourier coefficient bound for a cusp form](../../../../../../fourier-coefficient-bound-for-a-cusp-form.md) bounds these by $O(n^{k/2})$, but at arbitrarily large [primes](../../../../../../prime-number.md) $p$ their magnitude is $|a_1-a_0c_k|(1+p^{k-1})$. Since $k-1>k/2$, the coefficient factor must vanish. All coefficients of $h$ then vanish, including its constant coefficient, so $h=0$ by its cusp expansion and the [identity theorem](../../../../../../identity-theorem.md). This proves the [noncuspidal level-one Hecke eigenform](../../../../../../noncuspidal-level-one-hecke-eigenform.md) characterization:

$$
\boxed{f=a_0(f)E_k\qquad(k\geq4).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
