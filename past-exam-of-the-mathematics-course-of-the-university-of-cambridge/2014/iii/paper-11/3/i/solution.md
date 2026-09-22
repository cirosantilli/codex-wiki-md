<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Ahlswede–Daykin inequality](../../../../../../ahlswede-daykin-inequality.md), also called the [four functions theorem](../../../../../../ahlswede-daykin-inequality.md), concerns nonnegative functions $\alpha,\beta,\gamma,\delta$ on $\mathcal P([n])$. If

$$
\alpha(A)\beta(B)\le\gamma(A\cup B)\delta(A\cap B)\qquad\text{for all }A,B,
$$

then

$$
\boxed{\left(\sum_A\alpha(A)\right)\left(\sum_A\beta(A)\right)\le\left(\sum_A\gamma(A)\right)\left(\sum_A\delta(A)\right)}.
$$

Prove it by induction on $n$. The case $n=0$ is the single assumed inequality. For the induction step, sum each function over the last coordinate to obtain $\alpha',\beta',\gamma',\delta'$ on $\mathcal P([n-1])$. For fixed $A,B$ in this smaller cube, set $a_i=\alpha(A\cup i\{n\})$, $b_i=\beta(B\cup i\{n\})$, $c_i=\gamma((A\cup B)\cup i\{n\})$, and $d_i=\delta((A\cap B)\cup i\{n\})$, where $i\{n\}$ is empty for $i=0$ and $\{n\}$ for $i=1$.

The hypotheses give $a_0b_0\le c_0d_0$, $a_1b_1\le c_1d_1$ and $a_0b_1,a_1b_0\le c_1d_0$. The [two-point four-functions inequality](../../../../../../two-point-four-functions-inequality.md) shows that these imply $(a_0+a_1)(b_0+b_1)\le(c_0+c_1)(d_0+d_1)$. Here is its key algebra: put $x=a_0b_1$, $y=a_1b_0$, $M=c_1d_0$, $N=c_0d_1$. Then $x,y\le M$ and $xy\le MN$. If $M>0$, $(M-x)(M-y)\ge0$ gives $x+y\le M+xy/M\le M+N$; if $M=0$, both cross terms vanish. Adding the two diagonal bounds proves the claim.

Thus the primed functions satisfy the same hypothesis, and the induction hypothesis applies. Their totals equal the original totals, completing the proof.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
