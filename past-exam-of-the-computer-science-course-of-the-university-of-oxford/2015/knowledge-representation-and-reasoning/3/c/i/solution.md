<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use `not` for [negation as failure](../../../../../../negation-as-failure.md), rather than classical [logical negation](../../../../../../negation.md). The disjunctive condition is expressed by two separate [Datalog with negation](../../../../../../datalog-with-negation.md) rules:

$$
\boxed{\begin{aligned}
\mathit{Year}(x)\land\mathit{DivisibleBy}(x,400)&\to\mathit{Leap}(x),\\
\mathit{Year}(x)\land\mathit{DivisibleBy}(x,4)\land\operatorname{not}\mathit{DivisibleBy}(x,100)&\to\mathit{Leap}(x).
\end{aligned}}
$$

The positive $\mathit{Year}(x)$ premise restricts the rule to years and makes the variable explicitly safe. The divisibility relation is input data; the integer-looking constants do not make arbitrary arithmetic facts true automatically.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Knowledge representation and reasoning](../../../../knowledge-representation-and-reasoning-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
