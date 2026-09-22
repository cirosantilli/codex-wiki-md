<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $y=N^{1/\varphi(N)}$, $L=\sum_{p\le y}|g(p)|$, and $A=\sum_{p\le y}g(p)/p$. Put $I_p(n)=\mathbf1_{p\mid n}$ and $Y_p=I_p-1/p$. The [strongly additive arithmetic function](../../../../../../strongly-additive-arithmetic-function.md) identity is $g-A=\sum_{p\le y}g(p)Y_p$.

For any tuple $p_1,\ldots,p_j$, expand $\prod_{r=1}^j(I_{p_r}-1/p_r)$ by choosing an indicator in some positions and the constant in the others. If the selected positions contain distinct [primes](../../../../../../prime-number.md) whose product is $d$, then

$$
\mathbb E_N\prod_{r\text{ selected}}I_{p_r}=\frac{\lfloor N/d\rfloor}N=\frac1d+O(N^{-1}).
$$

For the corresponding product of the independent [Bernoulli random variables](../../../../../../bernoulli-distribution.md) $X_p$, the [expectation](../../../../../../expected-value.md) is exactly $1/d$. This includes repeated [primes](../../../../../../prime-number.md), since their [indicator functions](../../../../../../indicator-function.md) are idempotent, and the empty selection has zero error. Summing absolute values of all expansion coefficients bounds the difference by

$$
\frac1N\prod_{r=1}^j\left(1+\frac1{p_r}\right)\le\frac{2^j}{N}\le\frac{y^j}{N}
$$

when $y\ge2$. Expanding the $j$th power and summing the absolute coefficient weights gives

$$
\mathbb E_N(g-A)^j=\mathbb E\left(\sum_{p\le y}g(p)(X_p-1/p)\right)^j+O\left(\frac{y^jL^j}{N}\right).
$$

It remains to center at the actual [expectation](../../../../../../expected-value.md). Since $\mathbb E_N I_p=\lfloor N/p\rfloor/N$, we have $|\mathbb E_Ng-A|\le L/N$. For each $n$, both $g(n)-A$ and $g(n)-\mathbb E_Ng$ have absolute value at most $L$, because all their indicator coefficients have absolute value at most one. The identity $u^j-v^j=(u-v)\sum_{r=0}^{j-1}u^{j-1-r}v^r$ therefore bounds the change in the [central moment](../../../../../../central-moment.md) by $jL^j/N$.

Finally, [independence](../../../../../../independent-random-variables.md) factors each term of the independent [central moment](../../../../../../central-moment.md). If $q_1,\ldots,q_w$ are the distinct [primes](../../../../../../prime-number.md) of the tuple and $a_i$ their multiplicities, **the desired comparison** becomes

$$
\boxed{\mathbb E_N(g-\mathbb E_Ng)^j=\sum_{p_1,\ldots,p_j\le y}\prod_{i=1}^w g(q_i)^{a_i}\mathbb E(X_{q_i}-1/q_i)^{a_i}+O\left(\frac{j y^j}{N}L^j\right).}
$$

If $y<2$, then $g=0$ and both sides vanish, so the formula remains valid. The argument also covers complex coefficients $g(p)$; a real-valued assumption is needed for the later [normal distribution](../../../../../../normal-distribution.md) conclusion, not for this [centered moment comparison for additive arithmetic functions](../../../../../../centered-moment-comparison-for-additive-arithmetic-functions.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
