<h1 id="33c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $x=\mathcal E/(k_BT)>0$ and $r=e^{-x}$. The one-particle internal [partition function](../../../../../../canonical-partition-function.md) is $z=(1-r^q)/(1-r)$, and independence gives $Z=z^N$. The mean level index is

$$
\langle j\rangle=-\frac d{dx}\log z=\frac r{1-r}-\frac{qr^q}{1-r^q}.
$$

Thus the full internal entropy is

$$
\boxed{S=Nk_B\left[\log\frac{1-e^{-qx}}{1-e^{-x}}+
 x\left(\frac1{e^x-1}-\frac q{e^{qx}-1}\right)\right]}.
$$

This describes the specified internal degrees of freedom, with no translational or mixing contribution added. For a positive level spacing, **$S\to0$ as $T\to0$**, since the unique lowest internal level becomes certain, while **$S\to Nk_B\log q$ as $T\to\infty$**, since all $q^N$ internal configurations become equally likely. The formula includes $q=1$, where the entropy is identically zero.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [33C](../../33c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
