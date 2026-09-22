<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Compose the two assumed isomorphisms to obtain a membership-preserving and membership-reflecting [bijection](../../../../../bijection.md)

$$
f=\pi_2\circ\pi_1^{-1}:M_1\to M_2.
$$

Transitivity of both targets implies, for every $a\in M_1$,

$$
f(a)=\{f(b):b\in a\}.
$$

For one inclusion use preservation of membership. For the other, if $c\in f(a)$, transitivity puts $c$ in $M_2$; surjectivity gives $c=f(b)$ for $b\in M_1$, and reflection gives $b\in a$.

Apply the [membership induction theorem](../../../../../membership-induction-theorem.md) to the assertion that every $a\in M_1$ is fixed. If all members $b$ of $a$ are fixed, the displayed equation gives $f(a)=a$. Thus $f$ is the identity on $M_1$. Its range is $M_2$, so $M_1=M_2$, and the definition of $f$ gives

$$
\boxed{\pi_1=\pi_2,\qquad M_1=M_2.}
$$

This proves uniqueness of the [Mostowski collapse theorem](../../../../../mostowski-collapse-theorem.md). Existence of the two isomorphisms already supplies the membership structure needed in this argument.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
