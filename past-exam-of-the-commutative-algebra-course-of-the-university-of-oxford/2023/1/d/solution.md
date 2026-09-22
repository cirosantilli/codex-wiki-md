<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $A=\mathbb C[X,Y]$, $P=(X)$ and $Q=(X^2,Y)$. The [quotient ring](../../../../quotient-ring.md) $A/P\cong\mathbb C[Y]$ is an [integral domain](../../../../integral-domain.md), so $P$ is a [prime ideal](../../../../prime-ideal.md) and hence a [primary ideal](../../../../primary-ideal.md). Put $\mathfrak m=(X,Y)$. Then

$$
\mathfrak m^2=(X^2,XY,Y^2)\subseteq Q\subseteq\mathfrak m.
$$

The [polynomial ring](../../../../polynomial-ring.md) $A$ is a [Noetherian ring](../../../../noetherian-ring.md) by the [Hilbert basis theorem](../../../../hilbert-basis-theorem.md), and $\mathfrak m$ is a [maximal ideal](../../../../maximal-ideal.md) since $A/\mathfrak m\cong\mathbb C$. Therefore the [maximal-primary ideal criterion](../../../../maximal-primary-ideal-criterion.md) from [c](../c.md) makes $Q$ $\mathfrak m$-[primary](../../../../primary-ideal.md). In particular its [radical of an ideal](../../../../radical-of-an-ideal.md) is $\mathfrak m$, distinct from $P$.

Neither [primary ideal](../../../../primary-ideal.md) can be omitted: $X\in P\setminus Q$, while $Y\in Q\setminus P$. Thus the given intersection is already a [minimal primary decomposition](../../../../minimal-primary-decomposition.md). To express the [ideal](../../../../ideal.md) by generators, write an element of $P\cap Q$ as $Xh=X^2u+Yv$. Reducing modulo the [prime ideal](../../../../prime-ideal.md) $(X)$ gives $Y\bar v=0$ in the [integral domain](../../../../integral-domain.md) $\mathbb C[Y]$, so $v=Xw$. Cancelling $X$ in the [integral domain](../../../../integral-domain.md) $A$ gives $h=Xu+Yw$. Hence

$$
\boxed{J=(X^2,XY)=(X)\cap(X^2,Y).}
$$

By the [first uniqueness theorem for primary decomposition](../../../../first-uniqueness-theorem-for-primary-decomposition.md), the [associated primes of a module](../../../../associated-prime-of-a-module.md) $A/J$ are exactly the two [radicals of ideals](../../../../radical-of-an-ideal.md). Their strict inclusion $P\subsetneq\mathfrak m$ gives

$$
\boxed{\operatorname{Ass}_A(A/J)=\{(X),(X,Y)\},\quad (X)\text{ isolated},\quad (X,Y)\text{ embedded}.}
$$

One can also see both [associated primes of a module](../../../../associated-prime-of-a-module.md) directly through [annihilators](../../../../annihilator-ring-theory.md):

$$
\operatorname{Ann}_A(Y+J)=(J:Y)=(X),\qquad
\operatorname{Ann}_A(X+J)=(J:X)=(X,Y).
$$

For the first [colon ideal](../../../../colon-ideal.md), reducing $hY\in J$ modulo $(X)$ forces $h\in(X)$, and the reverse inclusion follows from $XY\in J$. For the second [colon ideal](../../../../colon-ideal.md), cancel $X$ in $hX\in X(X,Y)$. Both represented elements of the [quotient module](../../../../quotient-module.md) $A/J$ are nonzero.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
