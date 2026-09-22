<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a single homogeneous equation

$$
c_1x_1+\cdots+c_rx_r=0
$$

with nonzero integer coefficients, [Rado theorem](../../../../../rado-s-theorem.md) says that it is a [partition regular equation](../../../../../partition-regular-equation.md) exactly when

$$
\sum_{i\in I}c_i=0
$$

for some nonempty $I\subseteq\{1,\ldots,r\}$.

For necessity, suppose no nonempty coefficient sum vanishes. Choose a prime $p$ dividing none of the finitely many nonzero numbers $\sum_{i\in I}c_i$. Colour $x\in\mathbb N$ by the first nonzero base-$p$ digit

$$
p^{-v_p(x)}x\pmod p.
$$

If $x_1,\ldots,x_r$ had one colour, divide the equation by the least power of $p$ occurring among them and reduce modulo $p$. The terms of minimum valuation give

$$
u\sum_{i\in I}c_i\equiv0\pmod p
$$

for a nonzero $u$, contradicting the choice of $p$.

For sufficiency, reorder so that $c_1+\cdots+c_t=0$. The standard focusing lemma derived from the [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md) says the following: given a finite colouring, a finite monochromatic solution of the first $j$ blocks of the columns condition can be chosen together with a common difference $d$ so that every bounded translate of every chosen entry by a multiple of $d$ retains its colour. To prove the lemma, refine the colour of $a$ to the finite vector $(\chi(a),\chi(2a),\ldots,\chi(Ra))$, apply van der Waerden to a sufficiently long progression in this refined colouring, and take a common multiple of the finitely many resulting coefficients as $d$.

Start with the zero-sum block $\{1,ldots,t\}$, for which equal variables already solve its contribution. Add each remaining coefficient as a singleton block. In one dimension its block sum is a rational multiple of any fixed nonzero earlier coefficient, so the focusing lemma chooses a bounded translate that cancels this new contribution while preserving the common colour. Induction over the remaining indices gives a monochromatic solution of the full equation. This proves the single-equation form of Rado's theorem.

Now let $a_1,ldots,a_n,b$ be positive and put $A=a_1+\cdots+a_n$. If $b=At$, then $x_1=\cdots=x_n=t$ is a monochromatic solution in every colouring. Conversely, every solution has $x_i\leq b/a_i$. Give each integer at most $b/\min_i a_i$ its own colour and colour all larger integers with one extra colour. A monochromatic solution must have all $x_i=t$, so $b=At$. Thus the inhomogeneous equation is partition regular exactly when $A$ divides $b$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 130](../../paper-130-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
