<h1 id="11e/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Set $F(h)=f(a+h)+f(a-h)-2f(a)$ and $G(h)=h^2$. Both vanish at zero. For $h\ne0$, their derivative ratio is

$$
\frac{F'(h)}{G'(h)}=\frac{f'(a+h)-f'(a-h)}{2h}
=\frac12\left(\frac{f'(a+h)-f'(a)}h+\frac{f'(a)-f'(a-h)}h\right).
$$

Twice [differentiability](../../../../../../differentiability.md) at $a$ makes both quotients tend to $f''(a)$. Apply the endpoint [L'Hôpital's rule](../../../../../../l-hopital-s-rule.md) proved in part (iii) for $h\downarrow0$. For the other side use the reflected positive variable $t=-h$; $F$ and $G$ are even, so their quotient is unchanged. Thus the two-sided limit is

$$
\boxed{\lim_{h\to0}\frac{f(a+h)+f(a-h)-2f(a)}{h^2}=f''(a).}
$$

This is the [second-order central difference](../../../../../../second-order-central-difference.md) limit. The proof only uses [differentiability](../../../../../../differentiability.md) of $f'$ at $a$ and [differentiability](../../../../../../differentiability.md) nearby; it does not incorrectly assume $f''$ is [continuous](../../../../../../continuous-function.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [11E](../../11e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
