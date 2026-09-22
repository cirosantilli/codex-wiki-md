<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [submodule](../../../../submodule.md) $N\subseteq M$, define its [subspace filtration](../../../../subspace-filtration.md) and the [quotient filtration](../../../../quotient-filtration.md) on the [quotient module](../../../../quotient-module.md) $Q=M/N$ by

$$
N_j=N\cap M_j,\qquad Q_j=(M_j+N)/N.
$$

They are compatible [filtrations of a module](../../../../filtration-of-a-module.md), since multiplication by $F_iR$ sends $N_j$ into $N_{i+j}$ and $Q_j$ into $Q_{i+j}$.

In each degree, inclusion and the quotient map induce

$$
\iota_j:N_j/N_{j-1}\longrightarrow M_j/M_{j-1},\qquad
\pi_j:M_j/M_{j-1}\longrightarrow Q_j/Q_{j-1}.
$$

The first map is [injective](../../../../injective-function.md): if $n\in N_j$ belongs to $M_{j-1}$, then $n\in N\cap M_{j-1}=N_{j-1}$. The second map is [surjective](../../../../surjective-function.md) by the definition of $Q_j$.

For exactness in the middle, a class $m+M_{j-1}$ lies in $\ker\pi_j$ precisely when $m\in M_j$ and $m+N\in Q_{j-1}$. This means $m=m'+n$ for $m'\in M_{j-1}$ and $n\in N$. Since $m,m'\in M_j$, one also has $n\in N_j$, and

$$
m+M_{j-1}=n+M_{j-1}\in\operatorname{im}\iota_j.
$$

Conversely, every class from $N_j$ maps to zero in $Q_j/Q_{j-1}$. Taking the [direct sum](../../../../direct-sum.md) over all degrees gives the [short exact sequence](../../../../short-exact-sequence.md) of [graded modules](../../../../graded-module.md)

$$
0\longrightarrow\operatorname{gr}N\longrightarrow\operatorname{gr}M
\longrightarrow\operatorname{gr}(M/N)\longrightarrow0.
$$

The maps respect the $\operatorname{gr}R$-action because they come from [module homomorphisms](../../../../module-homomorphism.md) compatible with the [filtrations of a module](../../../../filtration-of-a-module.md). Consequently

$$
\boxed{\operatorname{gr}M/\operatorname{gr}N\cong\operatorname{gr}(M/N)}
$$

as $\operatorname{gr}R$-[modules](../../../../module-mathematics.md). This proves [exactness of associated graded modules for induced filtrations](../../../../exactness-of-associated-graded-modules-for-induced-filtrations.md).

Furthermore $A=\operatorname{gr}R$ is a [Noetherian ring](../../../../noetherian-ring.md), and $\operatorname{gr}M$ is a [finitely generated module](../../../../finitely-generated-module.md). Its [submodule](../../../../submodule.md) $\operatorname{gr}N$ and its [quotient module](../../../../quotient-module.md) $\operatorname{gr}(M/N)$ are therefore [finitely generated modules](../../../../finitely-generated-module.md). Hence the induced [subspace filtration](../../../../subspace-filtration.md) and [quotient filtration](../../../../quotient-filtration.md) are both [good filtrations for the order filtration](../../../../good-filtration-for-the-order-filtration.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the non-commutative rings course of the University of Oxford](../../../split.md)
5. [Non-commutative rings course of the University of Oxford](../../../../non-commutative-rings-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
