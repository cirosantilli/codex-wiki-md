<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Begin with the variable [typing judgment](../../../../../typing-judgment.md) $\{x:A\}\mapsto x:A$. Because $z$ is absent from this [typing context](../../../../../typing-context.md), the [lambda abstraction](../../../../../lambda-abstraction.md) rule permits $z$ to have type $\star$:

$$
\frac{\{x:A\}\mapsto x:A}
{\{x:A\}\mapsto\lambda z.x:\star\Rightarrow A}.
$$

Assign the entire [lambda application](../../../../../lambda-application.md) $yx$ type $\star$ using the [universal typing axiom](../../../../../universal-typing-axiom.md), without attempting to assign a [function type](../../../../../function-type.md) to $y$. Then

$$
\frac{\{x:A\}\mapsto\lambda z.x:\star\Rightarrow A
\qquad\varnothing\mapsto yx:\star}
{\{x:A\}\mapsto(\lambda z.x)(yx):A}.
$$

Although $y$ is a [free variable](../../../../../free-variable.md) of the body, it is absent from its recorded [typing context](../../../../../typing-context.md). Consequently the [lambda abstraction](../../../../../lambda-abstraction.md) rule allows any [simple type](../../../../../simple-type.md) $B$ for $y$. Abstract over $y$ and then $x$:

$$
\frac{\displaystyle
\frac{\{x:A\}\mapsto(\lambda z.x)(yx):A}
{\{x:A\}\mapsto\lambda y.(\lambda z.x)(yx):B\Rightarrow A}}
{\varnothing\mapsto\lambda xy.(\lambda z.x)(yx):A\Rightarrow(B\Rightarrow A)}.
$$

The side condition for $y$ holds because $y$ is absent; the side condition for $x$ holds because its recorded [simple type](../../../../../simple-type.md) is $A$. Thus

$$
\boxed{\varnothing\mapsto\lambda xy.(\lambda z.x)(yx):A\Rightarrow(B\Rightarrow A)
\quad\text{for all }A,B\text{ in }\mathrm{TA}_\lambda^\star.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Lambda calculus and types](../../../lambda-calculus-and-types-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
