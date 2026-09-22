<h1 id="20f/solution">Solution</h1>

↑ **Parent:** [20F](../20f.md)

An algebraic number is an algebraic integer when it is a root of a monic [polynomial](../../../../../polynomial-split.md) in $\mathbb Z[X]$.

If $\alpha$ and $\beta$ are algebraic integers, the [ring](../../../../../ring.md) $\mathbb Z[\alpha,\beta]$ is a finitely generated $\mathbb Z$-module. Multiplication by $\alpha\beta$ preserves this module, so the [algebraic integer module criterion](../../../../../algebraic-integer-module-criterion.md) shows that $\alpha\beta$ is an algebraic integer.

The [ring of integers of a quadratic field](../../../../../ring-of-integers-of-a-quadratic-field.md) gives

$$
\mathcal O_{\mathbb Q(\sqrt2)}=\mathbb Z[\sqrt2],
$$

since $2\equiv2\pmod4$. For a direct verification, if $x=a+b\sqrt2$ with $a,b\in\mathbb Q$ is [integral](../../../../../integral.md), then its trace $2a$ and norm $a^2-2b^2$ are integers. Writing $2a=m\in\mathbb Z$ and reducing the norm condition in lowest terms shows first that $b$ can have denominator at most $2$; a denominator $2$ with odd numerator would require $m^2\equiv2\pmod4$, which is impossible. Thus $b\in\mathbb Z$, and then the norm condition forces $m$ even, so $a\in\mathbb Z$. Conversely, every $a+b\sqrt2$ with $a,b\in\mathbb Z$ is [integral](../../../../../integral.md) because $\sqrt2$ is [integral](../../../../../integral.md) and algebraic integers form a [ring](../../../../../ring.md).

Now let $f$ have degree $d$ and roots $\alpha_1,\ldots,\alpha_d$. Since

$$
2=M(f)=|a_d|\prod_j\max\{1,|\alpha_j|\}
$$

and $|\alpha_1|>1$, the integer $|a_d|$ cannot be $2$; hence $|a_d|=1$. Thus $f$ is monic up to sign and $\alpha_1$ is an algebraic integer.

Let $B$ be the product of all roots with [modulus](../../../../../modulus.md) greater than one, counting multiplicity. Complex roots occur in conjugate pairs, so $B$ is real up to the signs of the real roots and

$$
|B|=M(f)=2.
$$

As a product of algebraic integers, $B$ is an algebraic integer; the equality forces $B=\pm2$. Therefore

$$
\frac{|N_{\mathbb Q(\alpha_1)/\mathbb Q}(\alpha_1)|}{2}
$$

is the absolute value of the product of the remaining conjugates, is rational, and is an algebraic integer. It is consequently a nonzero rational integer. Every remaining factor has [modulus](../../../../../modulus.md) at most one, so this integer is at most one. It must equal one, and hence

$$
\boxed{|N_{\mathbb Q(\alpha_1)/\mathbb Q}(\alpha_1)|=2}.
$$

This is the [mahler-measure norm argument at measure two](../../../../../mahler-measure-norm-argument-at-measure-two.md).

## ↑ Ancestors (10)

1. [20F](../20f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
