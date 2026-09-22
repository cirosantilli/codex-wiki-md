<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the following fixed-number form of a logarithmic estimate: for chosen [logarithms](../../../../../logarithm.md) of fixed nonzero [algebraic numbers](../../../../../algebraic-number.md) $a_1,\ldots,a_s$, a nonzero form $\Lambda=\sum b_j\log a_j$ with [integer](../../../../../integer.md) coefficients $|b_j|\leq B$ satisfies $|\Lambda|\geq c(2B)^{-C}$, for fixed positive constants $c,C$. This follows from the [Baker lower bound for a homogeneous linear form in logarithms](../../../../../baker-lower-bound-for-a-homogeneous-linear-form-in-logarithms.md).

By the [Dirichlet unit theorem](../../../../../dirichlet-s-unit-theorem.md), write units as $x=\zeta\prod\epsilon_j^{m_j}$ and $y=\xi\prod\epsilon_j^{n_j}$, with finitely many [roots of unity](../../../../../root-of-unity.md) and fixed fundamental units. If the unit rank is zero, there are already only finitely many choices. Otherwise put $B=\max(1,|m_j|,|n_j|)$. The real logarithmic embedding of the free [unit group](../../../../../unit-group.md) has full rank and lies in the product-formula hyperplane. Equivalence of norms in that finite-dimensional space shows that a unit with exponent size $B$ has some archimedean conjugate of modulus at most $e^{-c_0B}$: a large positive logarithmic coordinate forces a comparably large negative one, and a large negative coordinate itself suffices.

Interchanging the two terms if necessary, choose such a conjugate for $y$. At this embedding the equation makes $\sigma(\alpha x)=1-\sigma(\beta y)$ with $|\sigma(\beta y)|\leq C_0e^{-c_0B}$. For large $B$ define the [logarithm](../../../../../logarithm.md) near one. It is nonzero because $\beta y\ne0$, and

$$
0<|\Lambda|=|\log(\sigma(\alpha x))|\leq2C_0e^{-c_0B}.
$$

On fixed branches it is

$$
\Lambda=\log\sigma(\alpha)+\log\sigma(\zeta)+\sum_jm_j\log\sigma(\epsilon_j)+2k\log(-1)
$$

for an [integer](../../../../../integer.md) $k=O(B)$. The bound on $k$ follows from summing the fixed imaginary parts and then reducing to the near-one branch. There are only finitely many possible embeddings and [roots of unity](../../../../../root-of-unity.md), so the stated lower bound applies uniformly with coefficients $O(B)$. It contradicts the exponential upper bound when $B$ is large. Hence the exponents are bounded and **$\boxed{\alpha x+\beta y=1\text{ has finitely many unit solutions}}$** in $\mathcal O_K^\times$. This is the [unit equation over a number field](../../../../../unit-equation-over-a-number-field.md) proof; “unit” here means an algebraic-[integer](../../../../../integer.md) unit, not an arbitrary nonzero field element.

For the [Thue theorem](../../../../../thue-theorem.md), let $F\in\mathbb Z[X,Y]$ be irreducible homogeneous of degree $d\geq3$ and let $m\ne0$ be fixed. In a [splitting field](../../../../../splitting-field.md) $L$, write $F(X,Y)=a\prod_i(X-\theta_iY)$ with distinct roots. Choose a fixed [integer](../../../../../integer.md) $c$ so that each $c\theta_i$ is integral and $c^dm/a$ is a nonzero [integer](../../../../../integer.md). For a solution $(u,v)$ the nonzero [algebraic integers](../../../../../algebraic-integer.md) $t_i=c(u-\theta_iv)$ satisfy $\prod_it_i=c^dm/a$. Their [principal ideals](../../../../../principal-ideal.md) therefore divide a fixed [ideal](../../../../../ideal.md) and have only finitely many possibilities. For each occurring [principal ideal](../../../../../principal-ideal.md) choose a generator $\gamma_i$, so $t_i=\gamma_i\varepsilon_i$ with $\varepsilon_i$ a unit.

Any three distinct roots give the identity

$$
(\theta_2-\theta_3)t_1+(\theta_3-\theta_1)t_2+(\theta_1-\theta_2)t_3=0.
$$

Divide by the third term and absorb the finitely many generator ratios into the coefficients. This is a fixed-coefficient unit equation in $\varepsilon_1/\varepsilon_3$ and $\varepsilon_2/\varepsilon_3$, so it has finitely many solutions for each generator choice. Thus $\rho=t_1/t_3$ has finitely many values. The relation $(1-\rho)u=(\theta_1-\rho\theta_3)v$ fixes a rational direction whenever an [integer](../../../../../integer.md) solution exists; $\rho=1$ simply gives $v=0$. On each such direction, $(u,v)=k(u_0,v_0)$ for a primitive [integer](../../../../../integer.md) pair, and $k^dF(u_0,v_0)=m$ allows finitely many $k$. This proves the desired finiteness. When $m=0$, irreducibility excludes a nonzero rational root direction, leaving only $(0,0)$.

The argument also proves finiteness for any [binary form](../../../../../binary-form.md) with at least three distinct projective roots: irreducibility was used only to guarantee distinct roots and to dispose of the zero-value case. A rational invertible change of variables can move every projective root away from infinity; after clearing its fixed denominators, the resulting pairs lie in an [integer](../../../../../integer.md) lattice and the same proof applies. This stronger nonzero-value version will apply to the binomial forms in question 6.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
