<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First the [C-star identity](../../../../../../c-star-identity.md) and [submultiplicativity](../../../../../../submultiplicativity.md) give $\|a\|^2=\|a^*a\|\le\|a^*\|\|a\|$, hence $\|a\|\le\|a^*\|$ when $a\ne0$. Applying this to $a^*$ gives equality, so the [involution](../../../../../../involution.md) is isometric and continuous. Also $\|1\|=\|1\|^2$ and $1\ne0$, yielding $\|1\|=1$.

For a [Normal element of a C-star algebra](../../../../../../normal-element-of-a-c-star-algebra.md) $x$, put $b=x^*x$, which is a [self-adjoint C-star element](../../../../../../hermitian-element-of-a-c-star-algebra.md). Normality gives $(x^*)^2x^2=b^2$, and the [C-star identity](../../../../../../c-star-identity.md) applied to $x^2$ and to $b$ gives

$$
\|x^2\|^2=\|(x^*)^2x^2\|=\|b^2\|=\|b\|^2=\|x\|^4.
$$

Thus $\|x^2\|=\|x\|^2$. Every power of $x$ is normal because $x$ commutes with $x^*$, so iteration yields

$$
\|x^{2^j}\|=\|x\|^{2^j}\qquad(j\ge0).
$$

The [spectral radius formula](../../../../../../spectral-radius-formula.md) has a limit along all positive integers, and along this subsequence its root [norms](../../../../../../norm.md) are exactly $\|x\|$. Therefore

$$
\boxed{r(x)=\|x\|.}
$$

This proves [spectral radius norm equality for normal elements](../../../../../../spectral-radius-norm-equality-for-normal-elements.md) directly from the defining [norm](../../../../../../norm.md) identity, rather than assuming a spectral representation in advance.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
