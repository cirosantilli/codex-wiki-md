<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Extend the [Dirichlet character](../../../../../dirichlet-character.md) $\chi$ periodically to all [integers](../../../../../integer.md), putting $\chi(n)=0$ when $(n,N)>1$. Its [Dirichlet L-function](../../../../../dirichlet-l-function.md), initially on $\operatorname{Re}s>1$, is

$$
\boxed{L(\chi,s)=\sum_{n\geq1}\chi(n)n^{-s}
=\prod_{p\nmid N}(1-\chi(p)p^{-s})^{-1}.}
$$

The [Euler product](../../../../../euler-product.md) follows from unique [prime factorization](../../../../../fundamental-theorem-of-arithmetic.md) and [absolute convergence](../../../../../absolute-convergence.md); a [Dirichlet character](../../../../../dirichlet-character.md) is completely multiplicative on this extension. Write $\chi_0$ for the [principal Dirichlet character](../../../../../principal-dirichlet-character.md), equal to one on units and zero elsewhere.

For a [nonprincipal Dirichlet character](../../../../../nonprincipal-dirichlet-character.md) $\chi$, [character orthogonality](../../../../../character-orthogonality.md) gives $\sum_{a=1}^N\chi(a)=0$. Explicitly, multiplication by a unit $u$ with $\chi(u)\ne1$ permutes the unit residues and multiplies this sum by $\chi(u)$, forcing it to vanish. For $t>0$ set

$$
H_\chi(t)=\sum_{n\geq1}\chi(n)e^{-nt}
=\frac{\sum_{a=1}^N\chi(a)e^{-at}}{1-e^{-Nt}}.
$$

The numerator is $O(t)$ at zero and the denominator is $Nt+O(t^2)$, so $H_\chi$ is bounded, indeed analytic, near zero; it decays exponentially at infinity. Initially for $\operatorname{Re}s>1$, [absolute convergence](../../../../../absolute-convergence.md) justifies

$$
\Gamma(s)L(\chi,s)=\int_0^\infty H_\chi(t)t^{s-1}\,dt.
$$

This [Mellin transform](../../../../../mellin-transform.md) integral is holomorphic for $\operatorname{Re}s>0$, locally uniformly in $s$, and division by the [Gamma function](../../../../../gamma-function.md) proves the requested [analytic continuation](../../../../../analytic-continuation.md) to the left of the line one.

In fact, the same argument proves [Mellin continuation of a nonprincipal Dirichlet L-function](../../../../../mellin-continuation-of-a-nonprincipal-dirichlet-l-function.md) to the entire plane. If $H_\chi(t)=\sum_{r=0}^M c_rt^r+O(t^{M+1})$ at zero, subtract this [Taylor polynomial](../../../../../taylor-polynomial.md) on $(0,1)$ and add its explicit integrals:

$$
\Gamma(s)L(\chi,s)=\int_1^\infty H_\chi(t)t^{s-1}\,dt
+\sum_{r=0}^M\frac{c_r}{s+r}
+\int_0^1\left(H_\chi(t)-\sum_{r=0}^M c_rt^r\right)t^{s-1}\,dt.
$$

The last integral is holomorphic on $\operatorname{Re}s>-M-1$. Its possible simple [poles](../../../../../pole.md) at nonpositive integers cancel against zeros of $1/\Gamma(s)$. Letting $M$ increase shows that $L(\chi,s)$ is an [entire function](../../../../../entire-function.md), without any primitivity assumption.

For real $s>1$, use the absolutely convergent [Euler product](../../../../../euler-product.md) logarithm

$$
B_\chi(s)=\sum_{p\nmid N}\sum_{m\geq1}\frac{\chi(p)^m}{mp^{ms}}
=F_\chi(s)+R_\chi(s),\qquad e^{B_\chi(s)}=L(\chi,s).
$$

The higher-power remainder has the uniform estimate

$$
|R_\chi(s)|\leq\sum_p\sum_{m\geq2}p^{-m}
=\sum_p\frac1{p(p-1)}\leq\sum_{n\geq2}\frac1{n(n-1)}=1.
$$

For a [nonprincipal Dirichlet character](../../../../../nonprincipal-dirichlet-character.md) $\chi$, invoke the allowed [nonvanishing of a nonprincipal Dirichlet L-function at one](../../../../../nonvanishing-of-a-nonprincipal-dirichlet-l-function-at-one.md). Its holomorphy and nonvanishing give a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) on a small disk about one. On the connected real interval $1<s<1+\eta$, $B_\chi(s)$ differs from this logarithm by a fixed element of $2\pi i\mathbb Z$: the difference is continuous with exponential one. Thus the [prime-character sum near one](../../../../../prime-character-sum-near-one.md) is bounded. This branch argument is needed for complex-valued [Dirichlet characters](../../../../../dirichlet-character.md).

For $\chi_0$,

$$
L(\chi_0,s)=\zeta(s)\prod_{p\mid N}(1-p^{-s}).
$$

The finite product has a positive limit as $s\downarrow1$, and the residue-one [pole](../../../../../pole.md) of the [Riemann zeta function](../../../../../riemann-zeta-function.md) gives

$$
\boxed{F_{\chi_0}(s)=\log\frac1{s-1}+O(1)\longrightarrow+\infty,
\qquad F_\chi(s)=O(1)\quad(\chi\ne\chi_0).}
$$

Here $O(1)$ for nonprincipal [Dirichlet characters](../../../../../dirichlet-character.md) means bounded complex magnitude.

Finally, for a [residue class](../../../../../residue-class.md) $a$ coprime to $N$, [Orthogonality of Dirichlet characters](../../../../../orthogonality-of-dirichlet-characters.md) gives

$$
\sum_{p\equiv a\pmod N}p^{-s}
=\frac1{\varphi(N)}\sum_{\chi\bmod N}\overline{\chi(a)}F_\chi(s)
=\frac1{\varphi(N)}\log\frac1{s-1}+O(1).
$$

Only [primes](../../../../../prime-number.md) not dividing $N$ occur, so the character orthogonality applies to every term. This sum diverges as $s\downarrow1$. A finite collection of [primes](../../../../../prime-number.md) would give a bounded sum, a contradiction. **Every reduced residue class contains infinitely many [primes](../../../../../prime-number.md).** This is the [Dirichlet theorem on primes in arithmetic progressions](../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md); the coprimality hypothesis is essential.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 137](../../paper-137-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
