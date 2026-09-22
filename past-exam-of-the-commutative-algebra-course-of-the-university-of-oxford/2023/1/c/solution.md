<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose first that $\mathfrak a$ is $\mathfrak m$-[primary](../../../../primary-ideal.md). Since $R$ is a [Noetherian ring](../../../../noetherian-ring.md), choose a finite [generating set of an ideal](../../../../generating-set-of-an-ideal.md) $\mathfrak m=(x_1,\ldots,x_d)$. The equality of [radicals of ideals](../../../../radical-of-an-ideal.md) $\sqrt{\mathfrak a}=\mathfrak m$ supplies positive integers $e_i$ with $x_i^{e_i}\in\mathfrak a$. Set

$$
n=1+\sum_{i=1}^d(e_i-1).
$$

Every product of $n$ generators has some $x_i$ appearing at least $e_i$ times. Such products generate the [product of ideals](../../../../product-of-ideals.md) $\mathfrak m^n$, so $\mathfrak m^n\subseteq\mathfrak a$. Also $\mathfrak a\subseteq\sqrt{\mathfrak a}=\mathfrak m$. If $\mathfrak m=0$, take $n=1$ directly.

Conversely, suppose $\mathfrak m^n\subseteq\mathfrak a\subseteq\mathfrak m$. Taking [radicals of ideals](../../../../radical-of-an-ideal.md) gives

$$
\mathfrak m=\sqrt{\mathfrak m^n}\subseteq\sqrt{\mathfrak a}\subseteq\mathfrak m.
$$

Hence $\sqrt{\mathfrak a}=\mathfrak m$. The only [maximal ideal](../../../../maximal-ideal.md) containing $\mathfrak a$ is $\mathfrak m$: any such [maximal ideal](../../../../maximal-ideal.md) contains $\sqrt{\mathfrak a}$ and therefore equals $\mathfrak m$. By the [correspondence theorem for ideals](../../../../correspondence-theorem-for-ideals.md), the [quotient ring](../../../../quotient-ring.md) $R/\mathfrak a$ is a [local ring](../../../../local-ring.md) with [maximal ideal](../../../../maximal-ideal.md) $\mathfrak m/\mathfrak a$. Every element outside this [maximal ideal](../../../../maximal-ideal.md) is a [unit](../../../../unit-in-a-ring.md).

If $ab\in\mathfrak a$ and $a\notin\mathfrak a$, then $b$ cannot be outside $\mathfrak m$, since multiplying by its inverse in the [quotient ring](../../../../quotient-ring.md) would give $a\in\mathfrak a$. Thus $b\in\mathfrak m$ and $b^n\in\mathfrak a$, proving the required [primary ideal](../../../../primary-ideal.md) condition. We have proved the [maximal-primary ideal criterion](../../../../maximal-primary-ideal-criterion.md)

$$
\boxed{\mathfrak a\text{ is }\mathfrak m\text{-primary}\iff\mathfrak m^n\subseteq\mathfrak a\subseteq\mathfrak m\text{ for some }n\geq1.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
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
