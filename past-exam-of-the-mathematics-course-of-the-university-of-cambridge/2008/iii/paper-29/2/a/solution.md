<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Non-Archimedean absolute value](../../../../../../non-archimedean-absolute-value.md) on a field is a function $|\cdot|:K\to\mathbb R_{\ge0}$ with $|x|=0$ exactly for $x=0$, $|xy|=|x||y|$, and the [ultrametric inequality](../../../../../../ultrametric-inequality.md) $|x+y|\le\max(|x|,|y|)$. It is nontrivial if some nonzero element has value different from one. [Equivalent absolute values](../../../../../../equivalent-absolute-values.md) induce the same topology; for nontrivial absolute values this is equivalent to $|x|_2=|x|_1^c$ for some $c>0$.

Here is also a proof of the latter equivalence in the case needed. A positive power plainly preserves the open neighborhoods of zero. Conversely, if the topologies coincide, then $|x|_1<1$ if and only if $x^n\to0$ in the first topology, hence if and only if $|x|_2<1$. Choose $a$ with $0<|a|_1<1$. For every $x\ne0$, $m\in\mathbb Z$ and $n\ge1$, whether $|x^n/a^m|<1$ agrees for the two values. Comparison with all rational numbers $m/n$ therefore identifies the two ratios $\log|x|_j/\log|a|_j$. Thus $|x|_2=|x|_1^c$ with $c=\log|a|_2/\log|a|_1>0$.

Now let $|\cdot|$ be nontrivial and non-Archimedean on $\mathbb Q$. Since $|1|=1$ and every positive integer is a sum of ones, $|n|\le1$ for every integer. If all nonzero integers had value one, multiplicativity would make the absolute value trivial on all rationals. Hence some integer has value less than one; its prime factorization shows that some prime $p$ has $|p|<1$.

There cannot be two distinct such primes $p,q$. A [Bezout identity](../../../../../../bezout-identity.md) $ap+bq=1$ with $a,b\in\mathbb Z$ would give

$$
1=|ap+bq|\le\max(|a||p|,|b||q|)\le\max(|p|,|q|)<1.
$$

Thus every other prime has value one. Prime factorization of the numerator and denominator of $x\in\mathbb Q^\times$ now gives

$$
|x|=|p|^{v_p(x)}=p^{-c v_p(x)}=|x|_p^c,\qquad c=-\frac{\log|p|}{\log p}>0.
$$

Conversely $|x|_p=p^{-v_p(x)}$ is multiplicative and satisfies the [ultrametric inequality](../../../../../../ultrametric-inequality.md), since $v_p(x+y)\ge\min(v_p(x),v_p(y))$. Distinct primes give inequivalent values: $p^m\to0$ for the $p$-adic absolute value but $|p^m|_q=1$ for $q\ne p$. We have proved the [non-Archimedean part of Ostrowski theorem](../../../../../../non-archimedean-part-of-ostrowski-theorem.md):

$$
\boxed{\text{The nontrivial non-Archimedean absolute values on }\mathbb Q\text{ are }|\cdot|_p^c,\quad p\text{ prime},\ c>0.}
$$

There is exactly one equivalence class for each prime.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
