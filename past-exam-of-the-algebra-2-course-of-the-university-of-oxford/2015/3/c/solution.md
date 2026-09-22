<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The nonzero [ideal](../../../../ideal.md) $\widetilde P$ is principal because $\mathbb Q[t]$ is a [principal ideal domain](../../../../principal-ideal-domain.md). Choose a nonzero generator $h\in\mathbb Q[t]$. Part (a) gives

$$
f=\frac{h}{c(h)}\in\mathbb Z[t],\qquad c(f)=1.
$$

The nonzero rational scalar $c(h)$ is a [unit](../../../../unit-in-a-ring.md) in $\mathbb Q[t]$, so this rescaling does not change the generated [principal ideal](../../../../principal-ideal.md):

$$
\boxed{\widetilde P=(f)_{\mathbb Q[t]},\qquad c(f)=1.}
$$

Part (b) now places $f$ in $P$, since $f\in\widetilde P\cap\mathbb Z[t]$. Thus $(f)_{\mathbb Z[t]}\subseteq P$.

For the reverse inclusion, let $g\in P$ be nonzero. The displayed equality supplies $q\in\mathbb Q[t]$ with $g=fq$. Multiplicativity of [rational polynomial content](../../../../rational-polynomial-content.md) gives

$$
c(g)=c(f)c(q)=c(q).
$$

Since $g$ has [integer](../../../../integer-split.md) coefficients, $c(g)$ is a positive [integer](../../../../integer-split.md). The normalization from part (a) gives $q/c(q)\in\mathbb Z[t]$, so multiplying it by the integer $c(q)=c(g)$ proves $q\in\mathbb Z[t]$. Consequently $g\in(f)_{\mathbb Z[t]}$. The zero [polynomial](../../../../polynomial-split.md) belongs as well, proving

$$
\boxed{P=(f)_{\mathbb Z[t]}.}
$$

This is the divisibility descent in [Gauss lemma for polynomials](../../../../gauss-lemma-for-polynomials.md): dividing an integer-coefficient [polynomial](../../../../polynomial-split.md) by a [primitive polynomial](../../../../primitive-polynomial.md) cannot introduce a denominator into an exact quotient. Here it yields the description of [prime ideals of the integer polynomial ring above zero](../../../../prime-ideals-of-the-integer-polynomial-ring-above-zero.md). The generator has positive [polynomial degree](../../../../degree-of-a-polynomial.md), since a primitive constant would be a [unit](../../../../unit-in-a-ring.md) and would put $1$ in $P$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the algebra 2 course of the University of Oxford](../../../split.md)
5. [Algebra 2 course of the University of Oxford](../../../../algebra-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
