<h1 id="20g/solution">Solution</h1>

↑ **Parent:** [20G](../20g.md)

First suppose $|\sigma_i(\alpha)|=1$ for every complex embedding. The coefficients of the monic polynomial

$$
P_m(T)=\prod_{i=1}^n(T-\sigma_i(\alpha^m))
$$

are rational algebraic integers and hence integers. They are uniformly bounded in $m$, because each is an elementary symmetric sum of numbers of modulus one. Only finitely many such integer polynomials can occur, so only finitely many algebraic integers $\alpha^m$ occur. Two powers coincide; since $\alpha\neq0$, this gives $\alpha^{r-s}=1$. Thus $\alpha$ is a [root of unity](../../../../../root-of-unity.md). This is [Kronecker theorem on algebraic integers in the unit disk](../../../../../kronecker-theorem-on-algebraic-integers-in-the-unit-disk.md).

The second printed assertion is literally false for $\alpha=0$. For the intended statement with $\alpha\neq0$, use the [Minkowski embedding](../../../../../minkowski-embedding-of-a-number-field.md): algebraic integers of $K$ form a lattice, so only finitely many have all conjugates of modulus at most $2$. A nonzero algebraic integer with every conjugate of modulus at most one has

$$
1\leq|N_{K/\mathbb Q}(\alpha)|leq1,
$$

so every conjugate has modulus one and the first part applies. Consequently every non-root in that finite box has $\max_i|\sigma_i(\alpha)|>1$. Choose $c>1$ no larger than the least of these finitely many maxima, taking $c=2$ if there are no non-roots. Then every nonzero $\alpha\in\mathcal O_K$ satisfying $|\sigma_i(\alpha)|<c$ for all $i$ is a root of unity.

[Dirichlet unit theorem](../../../../../dirichlet-s-unit-theorem.md) states that for signature $(r_1,r_2)$,

$$
\mathcal O_K^\times\cong\mu(K)\times\mathbb Z^{r_1+r_2-1},
$$

and the [logarithmic embedding of number field units](../../../../../logarithmic-embedding-of-number-field-units.md) maps the free part to a full lattice in the hyperplane where the weighted coordinate sum is zero.

For a real quadratic field, the roots of unity are $\{\pm1\}$ and the logarithms of positive units form a nonzero discrete subgroup $a\mathbb Z\subset\mathbb R$. Its smallest positive element is $\log\epsilon$ for a unit $\epsilon>1$. Given any positive unit $u>1$, choose $n$ so that $1\leq u\epsilon^{-n}<\epsilon$; minimality forces the quotient to be $1$. Applying signs and inverses shows

$$
\mathcal O_K^\times=\{\pm\epsilon^n:n\in\mathbb Z\}.
$$

Since $11\equiv3\pmod4$, the [ring of integers of a quadratic field](../../../../../ring-of-integers-of-a-quadratic-field.md) is $\mathbb Z[\sqrt{11}]$. A unit $a+b\sqrt{11}$ satisfies the [Pell equation](../../../../../pell-equation.md) $a^2-11b^2=\pm1$. The element

$$
10+3\sqrt{11}
$$

has norm $1$. To prove it is the smallest unit above one without invoking the continued-fraction algorithm, suppose $1<a+b\sqrt{11}<10+3\sqrt{11}$. Replacing by its inverse or negative if needed makes $b>0$, and the conjugate relation implies $b\sqrt{11}<(u+u^{-1})/2<10$, so $b\leq3$. For $b=1,2,3$, the numbers $11b^2\pm1$ are respectively

$$
10,12;qquad43,45;qquad98,100.
$$

Only the last list contains a square, namely $100=10^2$, which yields the endpoint itself. Hence no smaller unit exists and

$$
\boxed{\epsilon=10+3\sqrt{11}}.
$$

## ↑ Ancestors (10)

1. [20G](../20g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
