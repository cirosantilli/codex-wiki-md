<h1 id="1i/solution">Solution</h1>

↑ **Parent:** [1I](../1i.md)

If the positive [odd integer](../../../../../odd-integer.md) $n$ has [prime factorization](../../../../../fundamental-theorem-of-arithmetic.md)

$$
n=\prod_{r=1}^s p_r^{e_r},
$$

its [Jacobi symbol](../../../../../jacobi-symbol.md) is

$$
\left(\frac an\right)=\prod_{r=1}^s\left(\frac a{p_r}\right)^{e_r},
$$

where each factor is a [Legendre symbol](../../../../../legendre-symbol.md); by convention $(a/1)=1$. Thus the symbol is zero exactly when $\gcd(a,n)>1$.

The [quadratic reciprocity](../../../../../quadratic-reciprocity.md) law for the [Jacobi symbol](../../../../../jacobi-symbol.md) says that for coprime positive odd integers $m,n$,

$$
\boxed{\left(\frac mn\right)\left(\frac nm\right)=(-1)^{(m-1)(n-1)/4}.}
$$

To prove it, write $m=\prod_i p_i^{e_i}$ and $n=\prod_jq_j^{f_j}$. The [quadratic reciprocity](../../../../../quadratic-reciprocity.md) law for distinct odd primes states

$$
\left(\frac{p_i}{q_j}\right)\left(\frac{q_j}{p_i}\right)
=(-1)^{(p_i-1)(q_j-1)/4}.
$$

Multiplying this identity over $i,j$ with multiplicities $e_i f_j$ gives the required product of [Jacobi symbols](../../../../../jacobi-symbol.md). Its sign exponent modulo two is

$$
\left(\sum_i e_i\frac{p_i-1}{2}\right)
\left(\sum_j f_j\frac{q_j-1}{2}\right)
\equiv \frac{m-1}{2}\frac{n-1}{2}\pmod2,
$$

because multiplication of odd integers adds the quantities $(r-1)/2$ modulo two. This proves the law.

For the requested value, two applications of reciprocity give

$$
\left(\frac{503}{2019}\right)
=-\left(\frac7{503}\right)
=\left(\frac6{7}\right)
=-1,
$$

since $2019\equiv7\pmod{503}$, $503\equiv6\pmod7$, and $6$ is a [quadratic nonresidue](../../../../../quadratic-nonresidue.md) modulo $7$.

## ↑ Ancestors (10)

1. [1I](../1i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
