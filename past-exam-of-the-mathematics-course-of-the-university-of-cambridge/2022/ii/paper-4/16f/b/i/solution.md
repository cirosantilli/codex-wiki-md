<h1 id="16f/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A relation $r$ on a set $x$ is [well-founded](../../../../../../../well-founded-relation.md) when every nonempty subset of $x$ has an $r$-minimal element. It is [extensional](../../../../../../../extensional-relation.md) when distinct elements have distinct predecessor sets:

$$
a\ne b
\Longrightarrow
\{z\in x:z\,r\,a\}
\ne
\{z\in x:z\,r\,b\}.
$$

The [Mostowski collapse theorem](../../../../../../../mostowski-collapse-theorem.md) states that every well-founded extensional relation on a set is uniquely isomorphic to membership on a transitive set; the collapse is recursively

$$
\pi(a)=\{\pi(b):b\,r\,a\}.
$$

For the requested example, let $A=V_{\omega+1}$ and define

$$
x_0=A,
\qquad
x_n=A\cup\{x_0,\ldots,x_{n-1}\}\quad(n\geq1),
\qquad
x=\{x_n:n\in\omega\}.
$$

No $x_n$ belongs to $A$, and therefore

$$
x_m\in x_n\quad\Longleftrightarrow\quad m<n.
$$

The map $x_n\mapsto n$ is an isomorphism from membership on $x$ to membership on the von Neumann ordinal $\omega$, so the Mostowski collapse is $\omega$. On the other hand, $x_0=V_{\omega+1}$ already has rank $\omega+1$, and hence the rank of $x$ is greater than $\omega$.

For statement (i), suppose $(x,r)$ is isomorphic to $(y,\in)$ with $y$ transitive. Membership is well-founded by the axiom of foundation. It is extensional on $y$ because transitivity ensures that the predecessors in $y$ of an element $a\in y$ are exactly the elements of $a$, and the axiom of extensionality distinguishes different sets. Both properties are preserved by isomorphism. Thus (i) is always true.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [16F](../../../16f.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
