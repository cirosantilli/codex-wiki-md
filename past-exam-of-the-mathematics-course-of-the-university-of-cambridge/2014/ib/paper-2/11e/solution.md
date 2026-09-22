<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

Let $D$ be a finite [integral domain](../../../../../integral-domain.md). For any $a\ne0$, multiplication $m_a:D\to D$ is injective: $ax=ay$ implies $a(x-y)=0$, hence $x=y$ because there are no zero divisors. An injective map of a finite set to itself is surjective, so $ab=1$ for some $b$. Every nonzero element is invertible; therefore **a finite integral domain is a field**.

For an [irreducible polynomial](../../../../../irreducible-polynomial.md) $f\in F[X]$, consider a nonzero class $[g]$ in the [quotient ring](../../../../../quotient-ring.md) $F[X]/(f)$. Since $f$ does not divide $g$, irreducibility gives $\gcd(f,g)=1$. The [Euclidean algorithm](../../../../../euclidean-algorithm.md) in the [polynomial ring](../../../../../polynomial-ring.md) gives polynomials $u,v$ with $uf+vg=1$. Modulo $(f)$, $[v][g]=1$. Thus **the quotient by an irreducible polynomial is a field**.

For a [field with four elements](../../../../../field-with-four-elements.md), use

$$
\boxed{\mathbb F_4=\mathbb F_2[X]/(X^2+X+1).}
$$

The quadratic has no root in $\mathbb F_2$, so is irreducible. Write $\alpha=[X]$. Polynomial division shows the elements are $0,1,\alpha,\alpha+1$, with $\alpha^2=\alpha+1$. Its multiplication table is

$$
\begin{array}{c|cccc}
\cdot&0&1&\alpha&\alpha+1\\ \hline
0&0&0&0&0\\
1&0&1&\alpha&\alpha+1\\
\alpha&0&\alpha&\alpha+1&1\\
\alpha+1&0&\alpha+1&1&\alpha
\end{array}
$$

For a [field with nine elements](../../../../../field-with-nine-elements.md), use

$$
\boxed{\mathbb F_9=\mathbb F_3[X]/(X^2+1).}
$$

The values of $X^2+1$ at $0,1,2$ are $1,2,2$, so the quadratic is irreducible. Every class is uniquely $a+b\beta$, $a,b\in\mathbb F_3$, with $\beta^2=-1=2$. These nine classes form a [finite field](../../../../../finite-field.md); multiplication is $(a+b\beta)(c+d\beta)=(ac-bd)+(ad+bc)\beta$, with coefficients modulo three.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
