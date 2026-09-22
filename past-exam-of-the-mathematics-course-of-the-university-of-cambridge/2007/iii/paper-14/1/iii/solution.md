<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [alternating dyadic colouring excludes symmetric weighted pair sums](../../../../../../alternating-dyadic-colouring-excludes-symmetric-weighted-pair-sums.md) construction:

$$
\boxed{c(n)=\lfloor\log_2 n\rfloor\pmod2.}
$$

Thus consecutive [dyadic intervals](../../../../../../dyadic-interval.md) $[2^k,2^{k+1})$ have opposite colours. Suppose an increasing infinite [sequence](../../../../../../sequence.md) $X=(x_j)$ had all its distinct-index weighted sums in one [colour class](../../../../../../colour-class.md). [Set](../../../../../../set-split.md) $\delta(y)=2^{\lfloor\log_2 y\rfloor+1}-y$, the distance to the next strictly larger power of $2$.

If $\delta$ is unbounded on $X$, fix a term $x$ and choose a later term $y>2x$ with $\delta(y)>2x$. Put $L=2^{\lfloor\log_2 y\rfloor}$, so $y=2L-\delta(y)$. Then

$$
L\le y+2x<2L,\qquad 2L\le2y+x=4L-2\delta(y)+x<4L.
$$

These two weighted sums lie in adjacent [dyadic intervals](../../../../../../dyadic-interval.md) and therefore have opposite colours.

If $\delta$ is bounded by $D$ on $X$, choose a term $x>2D$ and a later term $y>2x$. With the same $L$, we have

$$
2L<y+2x=2L-\delta(y)+2x<4L,
\qquad
4L<2y+x=4L-2\delta(y)+x<8L.
$$

For the upper bounds, $y+2x<2y<4L$ and $2y+x<\tfrac52y<5L<8L$. These weighted sums also lie in adjacent [dyadic intervals](../../../../../../dyadic-interval.md). In both cases they are $x_i+2x_j$ and $x_j+2x_i$ for two distinct indices, contradicting the common [colour class](../../../../../../colour-class.md). Hence **the symmetric distinct-index conclusion is false**, even for this two-colour [finite colouring](../../../../../../finite-coloring.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
