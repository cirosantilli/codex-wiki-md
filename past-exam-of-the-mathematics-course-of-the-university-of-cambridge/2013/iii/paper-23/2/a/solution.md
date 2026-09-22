<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [even Dirichlet character](../../../../../../even-dirichlet-character.md) satisfies $\chi(-1)=1$, while an [odd Dirichlet character](../../../../../../odd-dirichlet-character.md) satisfies $\chi(-1)=-1$. Write $a=0$ or $1$ for its [character parity](../../../../../../character-parity.md) and, for $x>0$, define the [Dirichlet character theta function](../../../../../../dirichlet-character-theta-function.md)

$$
\theta_\chi(x)=\sum_{n\in\mathbb Z}n^a\chi(n)e^{-\pi n^2x/q}.
$$

For a [primitive Dirichlet character](../../../../../../primitive-dirichlet-character.md) whose [conductor of a Dirichlet character](../../../../../../conductor-of-a-dirichlet-character.md) is $q>1$, the term at zero is zero. Put $\tau(\chi)=\sum_{r\bmod q}\chi(r)e(r/q)$, using the positive exponential, and $\varepsilon_\chi=\tau(\chi)/(i^a\sqrt q)$. The primitive [Gauss sum of a Dirichlet character](../../../../../../gauss-sum-of-a-dirichlet-character.md) has magnitude $\sqrt q$, so $|\varepsilon_\chi|=1$. The theta transformation is

$$
\boxed{\theta_\chi(x)=\varepsilon_\chi x^{-a-1/2}\theta_{\overline\chi}(1/x).}
$$

Thus the powers are $x^{-1/2}$ in the even case and $x^{-3/2}$ in the odd case; the odd root number contains $1/i$. The conjugate character is necessary for a nonreal character. These formulas also follow by applying [Poisson summation](../../../../../../poisson-summation-formula.md) to the [Gaussian function](../../../../../../gaussian-function.md) on each [residue class](../../../../../../residue-class.md), and to its derivative for odd parity. For the primitive [principal Dirichlet character](../../../../../../principal-dirichlet-character.md) whose [conductor of a Dirichlet character](../../../../../../conductor-of-a-dirichlet-character.md) is one, use the ordinary [Jacobi theta function](../../../../../../jacobi-theta-function.md) with constant term one; its transformation has root number one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
