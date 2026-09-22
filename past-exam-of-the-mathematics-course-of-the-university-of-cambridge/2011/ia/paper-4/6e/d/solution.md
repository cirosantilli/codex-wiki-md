<h1 id="6e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Factor the equation as

$$
x^3+1=(x+1)(x^2-x+1).
$$

For the nontrivial roots, the [quadratic formula](../../../../../../quadratic-formula.md) over residues gives

$$
x=\frac{1\pm\sqrt{-3}}2\pmod{199}.
$$

The supplied square root is $14$, and $2^{-1}\equiv100\pmod{199}$. Therefore

$$
\boxed{x\equiv(1+14)100\equiv107\pmod{199}.}
$$

Indeed $107^2-107+1=11343=57\cdot199$, so $107^3+1$ is divisible by $199$, and $107\not\equiv-1$. The other nontrivial root is $(1-14)100\equiv93$; it satisfies $93^2-93+1=43\cdot199$. Together with $198\equiv-1$, these are the three cube roots of minus one. The complex-number hint reflects the same quadratic factor: the two roots there are $(1\pm\sqrt{-3})/2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
