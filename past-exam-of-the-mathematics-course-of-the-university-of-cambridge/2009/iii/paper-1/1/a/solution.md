<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\pi:G\to G/K$ be the [quotient group](../../../../../../quotient-group.md) homomorphism. Its restriction to $X$ is injective because its kernel there is $K\cap X=\{1\}$. Since $g\in K$, $\pi(x_ig)=\pi(x_i)$ for every generator. Let $F_n$ be the abstract [free group](../../../../../../free-group.md) on letters $a_1,\ldots,a_n$ and define the surjective [group homomorphism](../../../../../../group-homomorphism.md) $\alpha:F_n\to\langle x_1g,\ldots,x_ng\rangle$ by $\alpha(a_i)=x_ig$. If $w\in\ker\alpha$, then

$$
1=\pi(\alpha(w))=w(\pi(x_1),\ldots,\pi(x_n)).
$$

Injectivity on $X$ implies $w(x_1,\ldots,x_n)=1$ in $X$. Those elements are a [free basis of a group](../../../../../../free-basis-of-a-group.md), so $w$ is the empty reduced word in $F_n$. Thus $\ker\alpha=\{1\}$. This is [freeness detected by a quotient](../../../../../../freeness-detected-by-a-quotient.md), and proves

$$
\boxed{\langle x_1g,\ldots,x_ng\rangle\cong F_n\quad\text{freely on the displayed generators}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
