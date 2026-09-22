<h1 id="4/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the six-dimensional [vector space](../../../../../vector-space-split.md) of real symmetric $3\times3$ [matrices](../../../../../matrix.md) as the target, rather than all nine matrix entries independently. Define

$$
F:M_3(\mathbb R)\longrightarrow\operatorname{Sym}_3(\mathbb R),\qquad F(A)=A^TJA-J.
$$

Its derivative is

$$
DF_A(H)=H^TJA+A^TJH.
$$

The given $J$ is symmetric with $J^2=I$. Every $A\in G$ is invertible, since taking determinants of $A^TJA=J$ gives $(\det A)^2=1$. For any symmetric target $S$, choose

$$
H=\tfrac12AJS.
$$

Then $A^TJH=\tfrac12JJS=S/2$, and its transpose is also $S/2$. Thus $DF_A(H)=S$ and the derivative is [surjective](../../../../../surjective-function.md) at every point of $G$.

The [regular level set theorem](../../../../../regular-level-set-theorem.md) now gives

$$
\boxed{\dim G=9-6=3.}
$$

It also proves smooth embeddedness in the entire ambient [vector space](../../../../../vector-space-split.md) of [matrices](../../../../../matrix.md). The target symmetry is what gives the correct codimension.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [E](../../e.md)
3. [4](../../../4.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
