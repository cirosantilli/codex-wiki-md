<h1 id="5e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

As printed, the claim is false: $70$ is 7-cyclic-divisible because its rotations are $70$ and $07=7$, but its digits are not all equal to $7$ and its length is not a multiple of $6$.

The standard rotation argument proves the likely intended statement. If an $L$-digit integer and all its rotations are divisible by $7$, then for each leading digit $a$,

$$
10c_j(n)-c_{j+1}(n)=a(10^L-1)
$$

is divisible by $7$. The [multiplicative order](../../../../../../multiplicative-order.md) of $10$ modulo $7$ is $6$. If $6\nmid L$, then $7\nmid10^L-1$, forcing every digit $a$ to be divisible by $7$, hence to be either $0$ or $7$. Thus the valid conclusion is:

$$
\boxed{\text{either every digit is }0\text{ or }7,
\quad\text{or }6\mid L.}
$$

The counterexample shows why “all its digits are equal to 7” cannot replace the first alternative.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
