<h1 id="20g/solution">Solution</h1>

↑ **Parent:** [20G](../20g.md)

There is an error in the printed request: the cubic is not irreducible at $n=2$, and three elements cannot be a field [basis](../../../../../basis.md) in that case. The integral-basis assertion is valid under the necessary hypothesis $[\mathbb Q(\alpha):\mathbb Q]=3$.

Under that hypothesis, $\alpha$ is an [algebraic integer](../../../../../algebraic-integer.md) and $\mathbb Z[\alpha]\subseteq\mathcal O_k$ has finite index $m$. Change of [basis](../../../../../basis.md) in the [trace pairing](../../../../../trace-pairing.md) gives the discriminant-index identity

$$
\Delta(1,\alpha,\alpha^2)=m^2\operatorname{disc}(\mathcal O_k).
$$

The [field discriminant](../../../../../field-discriminant.md) is an [integer](../../../../../integer.md). If the left side is square-free, $m^2$ cannot divide it unless $m=1$. Thus **$1,\alpha,\alpha^2$ is an [integral basis](../../../../../integral-basis.md) when the cubic is irreducible and its [discriminant](../../../../../discriminant.md) is square-free**.

For any root, $\alpha^3=n\alpha+1$ gives

$$
\alpha(\alpha-\beta)(\alpha-\gamma)=\alpha f'(\alpha)=3\alpha^3-n\alpha=2n\alpha+3.
$$

Since $\alpha+\beta+\gamma=0$, $\alpha\beta+\beta\gamma+\gamma\alpha=-n$ and $\alpha\beta\gamma=1$,

$$
\prod_{r\in\{\alpha,\beta,\gamma\}}(2nr+3)=27-12n^3+8n^3=27-4n^3.
$$

On the other hand, the product of $r f'(r)$ is $-\Delta$: the product of the roots is one, and each of the three unordered root pairs contributes a negative squared difference. Therefore, without needing irreducibility for this polynomial calculation,

$$
\boxed{\Delta=4n^3-27.}
$$

The three-root product is the [field norm](../../../../../field-norm.md) only when the cubic is the minimal polynomial.

At $n=1$, the polynomial has no rational root (the only candidates are $\pm1$), so it is irreducible, and its [discriminant](../../../../../discriminant.md) is $-23$. Hence **$1,\alpha,\alpha^2$ is an [integral basis](../../../../../integral-basis.md)**.

At $n=2$,

$$
x^3-2x-1=(x+1)(x^2-x-1).
$$

If $\alpha=-1$, then $k=\mathbb Q$ with [integral basis](../../../../../integral-basis.md) $\{1\}$. If $\alpha=(1\pm\sqrt5)/2$, then $k=\mathbb Q(\sqrt5)$ and **$\{1,\alpha\}$ is an [integral basis](../../../../../integral-basis.md)**, since this quadratic order has square-free [discriminant](../../../../../discriminant.md) five; also $\alpha^2=\alpha+1$. In neither case is the three-element list a [basis](../../../../../basis.md). Its [discriminant](../../../../../discriminant.md) five is instead that of the degree-three algebra $\mathbb Q[x]/(x^3-2x-1)$; a [basis](../../../../../basis.md) there does not repair the printed assertion about the field $k$.

## ↑ Ancestors (10)

1. [20G](../20g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
