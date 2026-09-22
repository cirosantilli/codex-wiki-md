<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [integral domain](../../../../../integral-domain.md) $A$ is an [integrally closed domain](../../../../../integrally-closed-domain.md) if every element of its [fraction field](../../../../../field-of-fractions.md) which is an [integral element](../../../../../integral-element.md) over $A$ belongs to $A$. Explicitly, if $z\in\operatorname{Frac}A$ satisfies

$$
z^d+a_{d-1}z^{d-1}+\cdots+a_0=0,\qquad a_i\in A,
$$

then $z\in A$. Thus $\boxed{A\text{ is integrally closed exactly when its integral closure in its fraction field is }A}$.

Suppose $A$ is a [unique factorization domain](../../../../../unique-factorization-domain.md) and $z=a/b$ is integral, with $a,b\in A$, $b\ne0$, and with no common [irreducible element](../../../../../irreducible-element.md) as a factor. Multiplying its monic equation by $b^d$ gives

$$
a^d+a_{d-1}a^{d-1}b+\cdots+a_0b^d=0.
$$

Hence $b$ divides $a^d$. Every [irreducible element](../../../../../irreducible-element.md) dividing $b$ is a [prime element](../../../../../prime-element.md), so it would divide $a$, contrary to the choice of the fraction. Therefore $b$ is a [unit](../../../../../unit-in-a-ring.md), and $z\in A$. We have proved

$$
\boxed{\text{Every unique factorization domain is integrally closed}.}
$$

The [going-down theorem](../../../../../going-down-theorem.md) is the following. Let $A\subseteq B$ be an [integral extension](../../../../../integral-extension.md) of [integral domains](../../../../../integral-domain.md) with $A$ an [integrally closed domain](../../../../../integrally-closed-domain.md). If

$$
\mathfrak p_1\subseteq\mathfrak p_2\quad\text{in }A,\qquad
\mathfrak q_2\cap A=\mathfrak p_2\quad\text{for a prime ideal }\mathfrak q_2\subset B,
$$

then

$$
\boxed{\text{there is a prime ideal }\mathfrak q_1\subseteq\mathfrak q_2\text{ with }\mathfrak q_1\cap A=\mathfrak p_1.}
$$

We first prove this for a [module-finite ring extension](../../../../../module-finite-ring-extension.md) and then remove that extra hypothesis. We use the [Lying-over theorem](../../../../../lying-over-theorem.md), the [going-up theorem](../../../../../going-up-theorem.md), and the [incomparability theorem for integral extensions](../../../../../incomparability-theorem-for-integral-extensions.md): primes exist over every base prime, prime chains can be extended upwards, and distinct primes over the same base prime cannot contain one another. The [going-up theorem](../../../../../going-up-theorem.md) follows by applying the [Lying-over theorem](../../../../../lying-over-theorem.md) to the quotient by the lower prime. These results concern arbitrary [integral extensions](../../../../../integral-extension.md); none assumes the [going-down theorem](../../../../../going-down-theorem.md).

For the finite case, let $K=\operatorname{Frac}A$ and $L=\operatorname{Frac}B$. Since $B$ is module-finite, $L/K$ is a [finite field extension](../../../../../finite-field-extension.md). Take a finite [normal field extension](../../../../../normal-extension.md) $E/K$ containing $L$, obtained as a [splitting field](../../../../../splitting-field.md) of the minimal polynomials of finitely many field generators. The extension $E/K$ need not be a [separable field extension](../../../../../separable-extension.md). Let $C$ be the [integral closure](../../../../../integral-closure.md) of $A$ in $E$. Then $B\subseteq C$, and $C$ is integral over both $A$ and $B$.

We need one auxiliary fact: the [finite group](../../../../../finite-group.md) $G=\operatorname{Aut}_K(E)$ acts transitively on the [prime ideals](../../../../../prime-ideal.md) of $C$ over any fixed [prime ideal](../../../../../prime-ideal.md) $\mathfrak p$ of $A$. First observe that an element $w\in E$ fixed by all of $G$ is a [purely inseparable algebraic element](../../../../../purely-inseparable-algebraic-element.md) over $K$. Indeed, all $K$-embeddings of $K(w)$ into an [algebraic closure](../../../../../algebraic-closure.md) extend to $K$-[automorphisms](../../../../../automorphism.md) of the [normal field extension](../../../../../normal-extension.md) $E$. Hence the [minimal polynomial of an algebraic element](../../../../../minimal-polynomial-of-an-algebraic-element.md) $w$ has only one distinct root. In [characteristic zero](../../../../../characteristic-zero.md) this says $w\in K$; in characteristic $p>0$ it says $w^{p^e}\in K$ for some $e\ge0$.

Now let $Q,Q'$ be primes of $C$ over $\mathfrak p$, and suppose $Q$ is different from every $\sigma(Q')$, $\sigma\in G$. By the [incomparability theorem for integral extensions](../../../../../incomparability-theorem-for-integral-extensions.md), $Q$ is contained in none of these conjugate primes. The [prime avoidance](../../../../../prime-avoidance.md) lemma supplies

$$
x\in Q\setminus\bigcup_{\sigma\in G}\sigma(Q').
$$

The product

$$
h=\prod_{\sigma\in G}\sigma(x)
$$

is fixed by $G$, is integral over $A$, and lies in $Q$ because one factor is $x$. Choose an exponent $e_0$ equal to $1$ in [characteristic zero](../../../../../characteristic-zero.md), or a power of $p$ in characteristic $p$, such that $h^{e_0}\in K$. Since $A$ is an [integrally closed domain](../../../../../integrally-closed-domain.md), $h^{e_0}\in A$. It also lies in $Q\cap A=\mathfrak p$, hence in $Q'$. Because $Q'$ is a [prime ideal](../../../../../prime-ideal.md), some factor $\sigma(x)$ lies in $Q'$. This means $x\in\sigma^{-1}(Q')$, contradicting our choice. Thus $Q=\sigma(Q')$ for some $\sigma$, proving transitivity. The power $e_0$ accounts for the possible [purely inseparable field extension](../../../../../purely-inseparable-extension.md) and makes the argument valid in every characteristic.

Lift the prescribed $\mathfrak q_2$ to a prime $Q_2$ of $C$ by the [Lying-over theorem](../../../../../lying-over-theorem.md) for $B\subseteq C$. Separately, choose a prime $Q'_1$ over $\mathfrak p_1$ and use the [going-up theorem](../../../../../going-up-theorem.md) to find $Q'_2\supseteq Q'_1$ over $\mathfrak p_2$. Transitivity gives $\sigma\in G$ with $\sigma(Q'_2)=Q_2$. Then

$$
Q_1=\sigma(Q'_1)\subseteq Q_2,
\qquad Q_1\cap A=\mathfrak p_1.
$$

Contracting to $B$ gives $\mathfrak q_1=Q_1\cap B\subseteq\mathfrak q_2$ with the required contraction. This proves the [going-down theorem](../../../../../going-down-theorem.md) for the module-finite case.

For a general [integral extension](../../../../../integral-extension.md) $A\subseteq B$, consider $B_{\mathfrak q_2}$ and the [ideal](../../../../../ideal.md)

$$
J=\mathfrak p_1B_{\mathfrak q_2}.
$$

We claim that $J$ is disjoint from $A\setminus\mathfrak p_1$. Otherwise, clearing the finitely many denominators in an expression for an element $a\in J\cap(A\setminus\mathfrak p_1)$ gives

$$
s a=\sum_{i=1}^{h}a_i b_i,\qquad
s\in B\setminus\mathfrak q_2,\quad a_i\in\mathfrak p_1,\quad b_i\in B.
$$

The [subalgebra](../../../../../subalgebra.md) $B_0=A[s,b_1,\ldots,b_h]$ is a [module-finite ring extension](../../../../../module-finite-ring-extension.md) of $A$, since all its generators are [integral elements](../../../../../integral-element.md). Apply the finite case to $\mathfrak q_2\cap B_0$: there is a prime $Q_1\subseteq\mathfrak q_2\cap B_0$ contracting to $\mathfrak p_1$. The displayed identity puts $sa$ in $Q_1$, but $a\notin Q_1$. Thus $s\in Q_1\subseteq\mathfrak q_2$, a contradiction.

Localize $B_{\mathfrak q_2}$ further at the [multiplicative subset](../../../../../multiplicatively-closed-set.md) $A\setminus\mathfrak p_1$. The extension of $J$ is a proper [ideal](../../../../../ideal.md), by the disjointness just proved. Choose a [maximal ideal](../../../../../maximal-ideal.md) containing it and contract back to a [prime ideal](../../../../../prime-ideal.md) of $B_{\mathfrak q_2}$. This prime contains $J$ and avoids $A\setminus\mathfrak p_1$. Its contraction $\mathfrak q_1$ to $B$ lies inside $\mathfrak q_2$ by the [prime ideal correspondence for localization](../../../../../prime-ideal-correspondence-for-localization.md), and its contraction to $A$ is exactly $\mathfrak p_1$. This completes the proof of the [going-down theorem](../../../../../going-down-theorem.md) without any finite generation assumption on $B$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 101](../../paper-101-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
