<h1 id="6h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $k=m+1$ and $L=\lambda+X$. The posterior risk is

$$
\tfrac12\{e^{-ra}M(r)+e^{ra}M(-r)\},
$$

where $M(s)=(L/(L-s))^k$. Differentiating in $a$ gives

$$
e^{2ra}=\frac{M(r)}{M(-r)}=\left(\frac{L+r}{L-r}\right)^k.
$$

Thus

$$
\boxed{\hat\theta=\frac{m+1}{2r}\log\frac{\lambda+X+r}{\lambda+X-r}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6H](../../6h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
