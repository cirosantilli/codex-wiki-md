<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Read epsilon as actual set membership restricted to $X$, the interpretation in which ambient ZF makes the relation [well-founded](../../../../../well-founded-relation.md). The structure's [axiom of extensionality](../../../../../axiom-of-extensionality.md) assumption means

$$
x,x'\in X,\quad x\cap X=x'\cap X\quad\Longrightarrow\quad x=x'.
$$

By [well-founded recursion](../../../../../well-founded-recursion.md) on membership, define

$$
\boxed{\pi(x)=\{\pi(y):y\in x\cap X\}\qquad(x\in X).}
$$

The recursion theorem applies because the [Axiom of foundation](../../../../../axiom-of-regularity.md) makes the restricted relation [well-founded](../../../../../well-founded-relation.md) and each predecessor collection is a set. The [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) gives the set $M=\pi[X]$.

To prove injectivity, use membership induction on $x$ for the property that $x\in X$ and $\pi(x)=\pi(x')$ with $x'\in X$ imply $x=x'$. Suppose this property holds for every $y\in x\cap X$. Equality of the two images means that each $y\in x\cap X$ has some $y'\in x'\cap X$ with $\pi(y)=\pi(y')$, so the induction hypothesis gives $y=y'$. Conversely every $y'\in x'\cap X$ has the same image as some $y\in x\cap X$, and the same induction hypothesis again makes them equal. Hence $x\cap X=x'\cap X$, and the structure's [axiom of extensionality](../../../../../axiom-of-extensionality.md) gives $x=x'$.

The map is onto $M$ by definition. The recursion immediately preserves membership, and its injectivity makes membership reflection valid as well. Moreover if $z\in\pi(x)$ then $z=\pi(y)$ for a predecessor $y\in X$, so $z\in M$. Therefore $M$ is transitive and $\pi$ is the required membership isomorphism. This proves the existence direction of the [Mostowski collapse theorem](../../../../../mostowski-collapse-theorem.md).

**An arbitrary binary relation must also be [well-founded](../../../../../well-founded-relation.md).** [Axiom of extensionality](../../../../../axiom-of-extensionality.md) alone is insufficient in that interpretation: the one-element relation with a self-loop is extensional, but any collapse onto a [transitive set](../../../../../transitive-set.md) would produce a set containing itself, contrary to [Axiom of foundation](../../../../../axiom-of-regularity.md). The actual-membership interpretation above supplies precisely the hypothesis otherwise missing; no analogous claim is made for a general ill-founded relation.

## ↑ Ancestors (13)

1. [C](../c.md)
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
