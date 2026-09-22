<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

The rank is $r(\alpha)=\dim\operatorname{im}\alpha$ and the nullity is $n(\alpha)=\dim\ker\alpha$. Extending a basis of the kernel to a basis of $V$, the images of the added vectors form a basis of the image, proving the [rank-nullity theorem](../../../../../rank-nullity-theorem.md)

$$
\dim V=r(\alpha)+n(\alpha).
$$

Since $\operatorname{im}(\alpha+\beta)\subseteq\operatorname{im}\alpha+\operatorname{im}\beta$, the upper sum bound follows. Applying it to $\alpha=(\alpha+\beta)-\beta$ and interchanging $\alpha,\beta$ gives the lower bound. For products, the image lies in $\operatorname{im}\alpha$ and is the image under $\alpha$ of $\operatorname{im}\beta$, giving the upper bound; rank-nullity on that restriction gives

$$
r(\alpha\beta)\geq r(\beta)-n(\alpha)=r(\alpha)+r(\beta)-n.
$$

All four bounds are sharp. In a fixed basis, nested diagonal projections attain the product upper bound; placing $\operatorname{im}\beta$ with the smallest possible intersection with $\ker\alpha$ attains its lower bound. Taking $\beta=-\alpha$ on a subspace of dimension $\min(r(\alpha),r(\beta))$ attains the sum lower bound, while choosing the two images in general position and avoiding cancellation attains the sum upper bound.

Both upper bounds need not be attainable simultaneously over every field. Over $\mathbb F_2$ with $n=1$ and both ranks one, necessarily $\alpha=\beta=I$. Then $r(\alpha\beta)=1$ but $r(\alpha+\beta)=0$, below its upper bound one.

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
