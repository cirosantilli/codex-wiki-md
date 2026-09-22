<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [universal typing axiom](../../../../../universal-typing-axiom.md) supplies $\varnothing\mapsto q:\star$ for every [lambda term](../../../../../lambda-term.md) $q$. Use this as the argument premise of the [lambda application](../../../../../lambda-application.md) rule. The empty [typing context](../../../../../typing-context.md) is consistent with $\Gamma$, and its [union](../../../../../set-union.md) with $\Gamma$ is $\Gamma$:

$$
\frac{\Gamma\mapsto p:\star\Rightarrow A
\qquad \varnothing\mapsto q:\star}
{\Gamma\cup\varnothing\mapsto pq:A}.
$$

Hence

$$
\boxed{\Gamma\mapsto pq:A\quad\text{for every }q.}
$$

The [free variables](../../../../../free-variable.md) of $q$ need not appear in the resulting [typing context](../../../../../typing-context.md): the [universal typing axiom](../../../../../universal-typing-axiom.md) deliberately assigns $\star$ without recording them.

## ↑ Ancestors (11)

1. [A](../a.md)
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
