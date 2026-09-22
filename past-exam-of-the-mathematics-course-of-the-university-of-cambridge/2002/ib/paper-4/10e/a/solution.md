<h1 id="10e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By [equivalent norms](../../../../../../equivalent-norms.md), choose $c,C>0$ with $c\|h\|_1\le\|h\|_2\le C\|h\|_1$. Differentiability in the first [norm](../../../../../../norm.md) means that there is a bounded [linear map](../../../../../../linear-map.md) $L:V\to\mathbb R$ with $f(a+h)-f(a)-Lh=r(h)$ and $|r(h)|/\|h\|_1\to0$. The same $L$ is bounded in the second [norm](../../../../../../norm.md), since $|Lh|\le K\|h\|_1\le Kc^{-1}\|h\|_2$. Moreover,

$$
\frac{|r(h)|}{\|h\|_2}\le\frac1c\frac{|r(h)|}{\|h\|_1}\longrightarrow0.
$$

The two [norms](../../../../../../norm.md) define the same approach $h\to0$, so this proves differentiability with the same [Fréchet derivative](../../../../../../frechet-derivative.md) in the second [norm](../../../../../../norm.md). Reversing the [norms](../../../../../../norm.md) proves the converse.

For completeness, the [derivative](../../../../../../derivative.md) is unique: if $L_1,L_2$ both work, fix $v$ and take $h=tv$. The two remainder estimates imply $|(L_1-L_2)v|=o(1)$ as $t\to0$, so $(L_1-L_2)v=0$ for every $v$. Thus **differentiability and its [derivative](../../../../../../derivative.md) are independent of the chosen [norm](../../../../../../norm.md)**. This is [differentiability under equivalent norms](../../../../../../differentiability-under-equivalent-norms.md), not merely invariance of continuity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10E](../../10e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
