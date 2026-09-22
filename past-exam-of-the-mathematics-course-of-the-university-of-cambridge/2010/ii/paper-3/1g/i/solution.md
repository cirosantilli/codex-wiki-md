<h1 id="1g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $\alpha=\sqrt N$. Every positive solution satisfies

$$
0<\frac xy-\alpha=\frac{M}{y^2(x/y+\alpha)}<\frac1{2y^2}.
$$

After reducing $x/y=p/q$, we still have $|\alpha-p/q|<1/(2q^2)$. Here is the [continued fraction convergent](../../../../../../continued-fraction-convergent.md) criterion with its proof. If $p/q$ is reduced and obeys this inequality, it is a strict best approximation of the second kind: for any different $r/s$ with $0<s\le q$, the assumption $|s\alpha-r|\le|q\alpha-p|$ would give

$$
1\le|ps-qr|\le s|p-q\alpha|+q|r-s\alpha|<\frac{s+q}{2q}\le1,
$$

a contradiction. Choose consecutive [continued fraction convergents](../../../../../../continued-fraction-convergent.md) $p_j/q_j,p_{j+1}/q_{j+1}$ with $q_j\le q<q_{j+1}$. Their [determinant](../../../../../../determinant.md) is $\pm1$, their errors $e_j=q_j\alpha-p_j$ alternate in sign, and every [integer](../../../../../../integer.md) pair $(r,s)$ is uniquely $a(p_j,q_j)+b(p_{j+1},q_{j+1})$. For $0<s<q_{j+1}$, either $b=0$, or $a,b$ have opposite signs: positive $a,b$ would make $s\ge q_{j+1}$, negative $a,b$ make $s<0$, and $a=0$ is impossible. Opposite signs make $ae_j$ and $be_{j+1}$ have the same sign, so $|s\alpha-r|\ge|e_j|$. If $b=0$, reduction gives the $j$th convergent itself. Thus a strict best approximation must be a convergent. The [determinant](../../../../../../determinant.md) and alternating-error facts follow immediately from the recurrence $p_j=a_jp_{j-1}+p_{j-2}$, $q_j=a_jq_{j-1}+q_{j-2}$ and the positive continued-fraction tail formula. Therefore **the reduced ratio $x/y$ is a convergent of $\sqrt N$**. Without assuming $\gcd(x,y)=1$, the unreduced pair may be a common multiple of the convergent's numerator and denominator; for example $(10,2)$ for $N=24,M=4$ reduces to $5/1$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1G](../../1g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
