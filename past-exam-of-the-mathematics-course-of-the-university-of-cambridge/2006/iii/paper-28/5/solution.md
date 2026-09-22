<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Fix integers $q\ge1$ and $a$ with $(a,q)=1$. We prove the [Dirichlet theorem on primes in arithmetic progressions](../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md) by showing that the [prime](../../../../../prime-number.md) Dirichlet sum in this [residue class](../../../../../residue-class.md) diverges as its real exponent decreases to one.

First justify the required [Dirichlet L-function](../../../../../dirichlet-l-function.md) facts. If $\chi$ is a [nonprincipal Dirichlet character](../../../../../nonprincipal-dirichlet-character.md) modulo $q$, its sum over a full period is zero: choose a unit $b$ with $\chi(b)\ne1$, and multiplication by $b$ permutes the [residue classes](../../../../../residue-class.md), forcing the sum to equal $\chi(b)$ times itself. Therefore the partial sums $C_\chi(u)=\sum_{n\le u}\chi(n)$ are bounded by $q$. [Partial summation](../../../../../abel-s-summation-formula.md) gives

$$
L(s,\chi)=s\int_1^\infty C_\chi(u)u^{-s-1}\,du\qquad(\operatorname{Re}s>0),
$$

which supplies holomorphic continuation near one, with locally [uniform convergence](../../../../../uniform-convergence.md). For the [principal Dirichlet character](../../../../../principal-dirichlet-character.md) $\chi_0$,

$$
L(s,\chi_0)=\zeta(s)\prod_{p\mid q}(1-p^{-s})
$$

has a simple [pole](../../../../../pole.md) at one, with [residue](../../../../../residue.md) $\varphi(q)/q$.

The assumption in the question gives nonvanishing at one for real nonprincipal characters. We must also prove it for nonreal characters. For a nonreal $\chi$, its square $\chi^2$ is nonprincipal. For real $\sigma>1$, logarithms of the [Euler products](../../../../../euler-product.md) give

$$
\zeta(\sigma)^3|L(\sigma,\chi)|^4|L(\sigma,\chi^2)|\ge1.
$$

For a [prime](../../../../../prime-number.md) not dividing $q$, its logarithmic coefficient is $3+4\operatorname{Re}\chi(p)^k+\operatorname{Re}\chi(p)^{2k}=2(1+\cos\theta)^2\ge0$, where $\chi(p)^k=e^{i\theta}$. [Primes](../../../../../prime-number.md) dividing $q$ contribute only the positive zeta term. If $L(1,\chi)$ vanished to order $m\ge1$, the product would be $O((\sigma-1)^{4m-3})$ and tend to zero: the squared-character factor is bounded because $\chi^2$ is nonprincipal. This is a contradiction. Hence

$$
L(1,\chi)\ne0\qquad\text{for every nonprincipal }\chi.
$$

This step uses the given real-character hypothesis and the [Euler product positivity for L-function nonvanishing](../../../../../euler-product-positivity-for-l-function-nonvanishing.md) for all remaining characters.

In $\sigma>1$ choose the logarithm furnished by the absolutely convergent [Euler product](../../../../../euler-product.md). Its prime-power expansion gives

$$
\log L(\sigma,\chi)=\sum_p\frac{\chi(p)}{p^\sigma}+O(1).
$$

The error from powers $k\ge2$ is uniformly bounded as $\sigma\downarrow1$, by $\sum_p\sum_{k\ge2}1/(kp^{k\sigma})<\infty$. For nonprincipal $\chi$, nonvanishing and holomorphic continuation at one provide a bounded logarithm in a neighborhood of one. The Euler-product branch differs from that branch by a constant integral multiple of $2\pi i$ on the final real interval, so it too is bounded. Thus

$$
\sum_p\frac{\chi(p)}{p^\sigma}=O_q(1)\qquad(\chi\ne\chi_0).
$$

For the principal character, its simple [pole](../../../../../pole.md) instead gives

$$
\sum_{p\nmid q}\frac1{p^\sigma}=\log\frac1{\sigma-1}+O_q(1).
$$

The [Orthogonality of Dirichlet characters](../../../../../orthogonality-of-dirichlet-characters.md) gives, for [primes](../../../../../prime-number.md) not dividing $q$,

$$
1_{p\equiv a\pmod q}=\frac1{\varphi(q)}\sum_{\chi\bmod q}\overline{\chi(a)}\chi(p).
$$

Multiply by $p^{-\sigma}$ and sum. [Absolute convergence](../../../../../absolute-convergence.md) allows the interchange for $\sigma>1$, so

$$
\boxed{\sum_{p\equiv a\pmod q}\frac1{p^\sigma}=\frac1{\varphi(q)}\log\frac1{\sigma-1}+O_q(1).}
$$

The right side tends to infinity. If there were only finitely many [primes](../../../../../prime-number.md) in the progression, the left side would have a finite limit at one. This contradiction proves **infinitely many [primes](../../../../../prime-number.md) occur in every reduced [residue class](../../../../../residue-class.md)**. For $q=1$ or $2$ the character argument simply has no nonprincipal terms and gives the same conclusion.

For the final deduction the modulus $q$ is fixed. Let $A(t)=\pi(t;q,a)$. The given consequence of the [Siegel–Walfisz theorem](../../../../../siegel-walfisz-theorem.md) is $A(t)\sim t/(\varphi(q)\log t)$. [Partial summation](../../../../../abel-s-summation-formula.md), including the [prime](../../../../../prime-number.md) $2$ through the lower endpoint $2^-$ when appropriate, gives

$$
\sum_{\substack{p\le x\\p\equiv a\pmod q}}\frac1p=\frac{A(x)}x+\int_2^x\frac{A(t)}{t^2}\,dt.
$$

The boundary is $O_q(1/\log x)$. Write $A(t)=t(1+\varepsilon(t))/(\varphi(q)\log t)$ with $\varepsilon(t)\to0$. The main integral is $(\log\log x-\log\log2)/\varphi(q)$. The error is $o(\log\log x)$: given $\eta>0$, choose $T$ such that $|\varepsilon(t)|\le\eta$ for $t\ge T$. Its integral from $2$ to $T$ is a fixed constant, and its absolute value from $T$ to $x$ is at most $\eta\log\log x/\varphi(q)$ plus a fixed constant. Divide by $\log\log x$ and then let $\eta\downarrow0$. We obtain the [reciprocal primes in a fixed arithmetic progression](../../../../../reciprocal-primes-in-a-fixed-arithmetic-progression.md) asymptotic

$$
\boxed{\sum_{\substack{p\le x\\p\equiv a\pmod q}}\frac1p\sim\frac1{\varphi(q)}\log\log x.}
$$

The argument uses the supplied prime-counting asymptotic in this last part; the preceding infinitude proof did not assume the [Prime number theorem](../../../../../prime-number-theorem.md) in [arithmetic progressions](../../../../../arithmetic-progression.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
