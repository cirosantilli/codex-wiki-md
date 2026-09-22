<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

Multiplying the desired representation by $b_1b_2$ turns it into the integer equation

$$
a=a_1b_2+a_2b_1+nb_1b_2.
$$

Since $b_1$ and $b_2$ are [coprime integers](../../../../../coprime-integers.md), the necessary [modular multiplicative inverses](../../../../../modular-multiplicative-inverse.md) exist. Choose the unique representatives

$$
a_1\equiv a b_2^{-1}\pmod{b_1},\quad0\leq a_1<b_1,\qquad
a_2\equiv a b_1^{-1}\pmod{b_2},\quad0\leq a_2<b_2.
$$

Then $a-a_1b_2-a_2b_1$ is divisible by both $b_1$ and $b_2$, hence by their product, because they are [coprime](../../../../../coprime-integers.md). Defining

$$
n=\frac{a-a_1b_2-a_2b_1}{b_1b_2}
$$

therefore gives an integer and proves existence. Any other representation, reduced modulo $b_1$ and $b_2$, must have the same $a_1$ and $a_2$, since their allowed ranges contain exactly one representative of each residue. The integer equation then forces the same $n$. This proves uniqueness.

For the [prime-power fraction decomposition](../../../../../prime-power-fraction-decomposition.md), put $d_i=p_i^{n_i}$ and $B_i=b/d_i$. The distinct prime-power factors $d_i$ are pairwise [coprime](../../../../../coprime-integers.md), and $B_i$ has a [modular multiplicative inverse](../../../../../modular-multiplicative-inverse.md) modulo $d_i$. Define

$$
q_i\equiv aB_i^{-1}\pmod{d_i},\qquad0\leq q_i<d_i.
$$

Every term $q_jB_j$ with $j\ne i$ is divisible by $d_i$, while $q_iB_i\equiv a\pmod{d_i}$. Thus $a-\sum_iq_iB_i$ is divisible by all the pairwise coprime $d_i$ and therefore by $b$. With $n=(a-\sum_iq_iB_i)/b$, division by $b$ yields the required representation. Reducing any such representation modulo each $d_i$ proves uniqueness exactly as above. This is the residue-solving mechanism of the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md).

For $315=9\cdot5\cdot7$, the complementary factors are $35,63,45$. The required [modular inverses](../../../../../modular-multiplicative-inverse.md) give

$$
q_9=8,\qquad q_5=2,\qquad q_7=5,
$$

because $35\cdot8\equiv1\pmod9$, $63\cdot2\equiv1\pmod5$, and $45\cdot5\equiv1\pmod7$. Their numerator sum is $280+126+225=631=1+2\cdot315$. Thus **the unique decomposition** is

$$
\boxed{\frac1{315}=\frac89+\frac25+\frac57-2}.
$$

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
