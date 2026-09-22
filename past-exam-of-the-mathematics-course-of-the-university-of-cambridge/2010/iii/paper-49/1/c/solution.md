<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a [verified Grover promise test](../../../../../../verified-grover-promise-test.md). Since $n>1$, $N\geq4$. Choose

$$
k=\left\lfloor\frac\pi{4\theta}\right\rfloor,\qquad \theta=\arcsin(N^{-1/2}).
$$

This is a nearest integer to $\pi/(4\theta)-1/2$, so $|(2k+1)\theta-\pi/2|\leq\theta$. Run the [Grover search algorithm](../../../../../../grover-s-algorithm.md) for $k$ iterations and measure the candidate $x$. Make one further oracle query with input $|x\rangle|0\rangle$ and measure the answer bit $f(x)$. Declare that a marked entry exists exactly when this bit is one.

In the zero case the verification always returns zero, so the decision is correct with certainty. In the single-marked-entry case, verification returns one exactly when the candidate is $a$, and

$$
\mathbb P(\text{correct decision})
=\sin^2((2k+1)\theta)
\geq\cos^2\theta=1-\frac1N\geq\frac34.
$$

Finally, $\arcsin u\geq u$ on $[0,1]$ gives $k\leq\pi\sqrt N/4$. Hence

$$
\boxed{\text{success probability}\geq\frac34,\qquad\text{oracle calls}=k+1=O(\sqrt{2^n}).}
$$

The verification query is necessary for this decision rule: an unverified search-register label does not itself say whether it is marked.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
