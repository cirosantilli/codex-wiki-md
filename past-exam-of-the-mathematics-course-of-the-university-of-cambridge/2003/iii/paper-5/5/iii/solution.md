<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The answer is **exponential growth in the paper's coarse-equivalence sense**. Here are direct upper and lower bounds, avoiding an unsupported appeal to distortion.

Represent the generators by affine maps of the real line: $y(t)=t+1$ and $x(t)=t/3$. Then $x^{-1}yx(t)=t+3=y^3(t)$, so the defining [relator](../../../../../../relator.md) is respected. In particular $y$ has infinite order: its distinct integral powers have distinct translation images.

Given $k$ digits $d_j\in\{0,1,2\}$, define $m_0=0$, $m_{j+1}=3m_j+d_{j+1}$ and $W_0$ empty, $W_{j+1}=x^{-1}W_jxy^{d_{j+1}}$. Induction using the relation shows $W_j=y^{m_j}$ in the group. Each step increases word length by at most four, so $|W_k|\le4k$. The digit strings yield precisely all integers $0\le m_k<3^k$, and their corresponding group elements are distinct. Therefore

$$
\boxed{\beta(4k)\ge3^k,\qquad \beta(n)\ge3^{\lfloor n/4\rfloor}}.
$$

For the upper bound, in the four-letter symmetric alphabet $\{x,x^{-1},y,y^{-1}\}$ there are at most $4\cdot3^{j-1}$ freely reduced words of length $j\ge1$. Every element of the ball has such a representative, giving

$$
\boxed{\beta(n)\le1+4\sum_{j=1}^n3^{j-1}=2\cdot3^n-1}.
$$

These bounds prove the [exponential growth of the ternary affine Baumslag-Solitar group](../../../../../../exponential-growth-of-the-ternary-affine-baumslag-solitar-group.md) and show $\beta\sim_e(n\mapsto2^n)$, since positive exponential bases and constant rescalings of the argument give the same coarse class. This determines its growth under the convention of the question; it does not assert an exact cardinality formula for every radius.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
