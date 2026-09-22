<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

The [epsilon-recursion theorem](../../../../../epsilon-recursion-theorem.md) says that for every definable operation $G$ assigning a set $G(x,h)$ to each set $x$ and each function $h$ with domain $x$, there is a unique class function $F$ such that

$$
\boxed{F(x)=G(x,F\mathbin{\upharpoonright}x)}
$$

for every set $x$.

For uniqueness, suppose $F$ and $F'$ both satisfy the recursion. If they agree on every $y\in x$, then their restrictions to $x$ agree and hence

$$
F(x)=G(x,F\mathbin{\upharpoonright}x)
=G(x,F'\mathbin{\upharpoonright}x)=F'(x).
$$

The [epsilon induction](../../../../../epsilon-induction.md) principle therefore gives $F=F'$.

For existence, call a function $f$ coherent on a transitive set $T$ when

$$
f(z)=G(z,f\mathbin{\upharpoonright}z)\qquad(z\in T).
$$

The same epsilon-induction argument shows that any two coherent functions agree on the intersection of their transitive domains. Assuming coherent functions have been constructed below every member of $x$, their compatible union defines all values below $x$; adjoining the value prescribed by $G(x,\cdot)$ extends the construction to $x$. Epsilon induction establishes this construction for every $x$. The compatible local functions therefore unite to the required class function $F$.

A relation $r$ on $x$ is [well-founded](../../../../../well-founded-relation.md) when every nonempty subset of $x$ has an element with no $r$-predecessor in that subset. It is [extensional](../../../../../extensional-relation.md) when

$$
\{b:b\,r\,a\}=\{b:b\,r\,a'\}\quad\Longrightarrow\quad a=a'.
$$

The [Mostowski collapse theorem](../../../../../mostowski-collapse-theorem.md) states that every well-founded extensional relation $(x,r)$ is isomorphic to membership on a unique [transitive set](../../../../../transitive-set.md) $M$. Define recursively

$$
\pi(a)=\{\pi(b):b\,r\,a\}.
$$

Well-founded recursion makes $\pi$ well defined. Epsilon-style induction along $r$, together with extensionality, shows that $\pi$ is injective. By definition,

$$
b\,r\,a\iff\pi(b)\in\pi(a),
$$

so $\pi$ is an isomorphism from $(x,r)$ onto $(M,\in)$, where $M=\operatorname{ran}\pi$. If $z\in\pi(a)\in M$, then $z=\pi(b)$ for some $b\,r\,a$, so $z\in M$; hence $M$ is transitive. If another collapse $\pi'$ has transitive range, induction gives $\pi'(a)=\{\pi'(b):b\,r\,a\}=\pi(a)$, proving uniqueness.

Finally, suppose $x$ is finite. Its collapse $M$ is a finite transitive set, so every member of $M$ is [hereditarily finite](../../../../../hereditarily-finite-set.md). Therefore every well-founded extensional relation on $x$ collapses to a transitive subset of $V_\omega$.

Conversely, let $x$ be infinite. Choose the initial infinite ordinal $\kappa$ equinumerous with $x$. The successor ordinal $\kappa+1$ has the same cardinality as $\kappa$. Pulling its membership relation back along a bijection $x\to\kappa+1$ gives a well-founded extensional relation on $x$ whose collapse is $\kappa+1$. But $\kappa\in\kappa+1$ is not hereditarily finite, so $\kappa+1\nsubseteq V_\omega$. Consequently,

$$
\boxed{\text{the required sets }x\text{ are exactly the finite sets}.}
$$

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
