<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $p\equiv1\pmod{20}$, put $\theta=\sqrt{-p}$. Since $-p\equiv3\pmod4$, the [ring of integers of a quadratic field](../../../../ring-of-integers-of-a-quadratic-field.md) formula gives $R=\mathbb Z[\theta]$. Modulo five,

$$
X^2+p\equiv X^2+1=(X-2)(X+2).
$$

The two roots are distinct, so the [Dedekind factorization theorem](../../../../dedekind-factorization-theorem.md) gives

$$
(5)=P\overline P,\qquad
P=(5,\theta-2),\quad\overline P=(5,\theta+2),\quad
N(P)=N(\overline P)=5.
$$

In particular $P\ne\overline P$.

We prove that $[P]$ has [order of a group element](../../../../order-of-a-group-element.md) greater than $n$. Suppose instead that $P^k$ is a [principal ideal](../../../../principal-ideal.md) for some $1\leq k\leq n$. Since $P^k\subseteq R$, its generator is in $R$: write $P^k=(a+b\theta)$ with $a,b\in\mathbb Z$. Taking [ideal norms](../../../../ideal-norm.md) gives the positive [field norm](../../../../field-norm.md)

$$
5^k=a^2+pb^2.
$$

But $5^k\leq5^n<p$, so $b=0$. Thus $a^2=5^k$, forcing $k$ to be even and $a=\pm5^{k/2}$. This would give

$$
P^k=(a)=(5)^{k/2}=P^{k/2}\overline P^{k/2},
$$

contrary to [unique factorization of ideals in a number field](../../../../unique-factorization-of-ideals-in-a-number-field.md) and $P\ne\overline P$. Consequently no such $k$ exists. The [finiteness of the ideal class group](../../../../finiteness-of-the-ideal-class-group.md) ensures that $[P]$ has finite [order of a group element](../../../../order-of-a-group-element.md), so

$$
\boxed{\operatorname{ord}([P])>n}.
$$

For every positive [integer](../../../../integer-split.md) $n$, the allowed infinitude of [prime numbers](../../../../prime-number-split.md) in the progression $1\pmod{20}$ supplies one larger than $5^n$. Applying the construction proves [unbounded element orders in imaginary quadratic ideal class groups](../../../../unbounded-element-orders-in-imaginary-quadratic-ideal-class-groups.md). In particular, this establishes elements of arbitrarily large [order of a group element](../../../../order-of-a-group-element.md), rather than merely unbounded [class numbers](../../../../class-number.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic number theory course of the University of Oxford](../../../split.md)
5. [Algebraic number theory course of the University of Oxford](../../../../algebraic-number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
