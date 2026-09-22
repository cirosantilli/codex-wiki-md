<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the defining property of the [Frobenius complement](../../../../../../frobenius-complement.md): $H\cap H^x=\{1\}$ whenever $x\notin H$. The [induced character](../../../../../../induced-character.md) formula, extended linearly to any [class function](../../../../../../class-function.md), is

$$
\theta^G(g)=\frac1{|H|}\sum_{x\in G:\ x^{-1}gx\in H}\theta(x^{-1}gx).
$$

For $h\in H\setminus\{1\}$, a summand requires $h\in H\cap xHx^{-1}$. The Frobenius intersection property forces $x\in H$. All $|H|$ remaining terms equal $\theta(h)$ since $\theta$ is a [class function](../../../../../../class-function.md) on $H$, so $\theta^G(h)=\theta(h)$. At the identity,

$$
\theta^G(1)=[G:H]\theta(1)=0=\theta(1).
$$

Together these give

$$
\boxed{(\theta^G)_H=\theta.}
$$

The zero identity value is essential: at nonidentity elements the intersection argument already gives the equality, whereas induction multiplies the identity value by the subgroup index.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
