<h1 id="9e/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Events $A$ and $B$ are [independent](../../../../../../../independent-events.md) when

$$
\mathbb P(A\cap B)=\mathbb P(A)\mathbb P(B).
$$

For a possible sum $2\leq t\leq12$, let $N_t$ be the number of ordered die pairs with sum $t$. Then

$$
\mathbb P(A_t)=\frac{N_t}{36},
\qquad
\mathbb P(B_i)=\frac16.
$$

If $t-i\in\{1,\ldots,6\}$, then $\mathbb P(A_t\cap B_i)=1/36$; otherwise it is zero. Independence for a possible sum therefore requires

$$
\frac1{36}=\frac{N_t}{216},
$$

so $N_t=6$. This occurs only for $t=7$, and then $7-i$ is valid for every $i=1,\ldots,6$. Thus

$$
\boxed{A_t\text{ and }B_i\text{ are independent exactly when }
t=7,\ 1\leq i\leq6}.
$$

If impossible sums are admitted as events of probability zero, they are trivially independent as well.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [9E](../../../9e.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
