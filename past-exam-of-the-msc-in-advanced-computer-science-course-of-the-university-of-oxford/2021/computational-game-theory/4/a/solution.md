<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**If the [core](../../../../../core-game-theory.md) is nonempty, it is exactly the singleton allocation $p_j=v(\{j\})$ for every $j$.** Take any $p$ in the [core of a cooperative game](../../../../../core-game-theory.md) and write $p(C)=\sum_{j\in C}p_j$. Core membership gives efficiency of the [imputation](../../../../../imputation-in-a-coalitional-game.md), $p(N)=v(N)$, and the [coalition](../../../../../coalition-game-theory.md) inequalities

$$
p(C)\ge v(C),\qquad p(N\setminus C)\ge v(N\setminus C).
$$

Using the given complementary-coalition equality in this [constant-sum cooperative game](../../../../../constant-sum-cooperative-game.md), the second inequality yields

$$
p(C)=v(N)-p(N\setminus C)
\le v(N)-v(N\setminus C)=v(C).
$$

Combining upper and lower bounds gives $p(C)=v(C)$ for every [coalition](../../../../../coalition-game-theory.md) $C$. In particular,

$$
\boxed{p_j=p(\{j\})=v(\{j\})\quad\text{for every }j\in N.}
$$

Since this holds for any [core](../../../../../core-game-theory.md) member and at least one exists by hypothesis, the displayed allocation is in the [core](../../../../../core-game-theory.md) and is its only member. The argument also shows why nonemptiness is restrictive: it forces $v(C)=\sum_{j\in C}v(\{j\})$ for every [coalition](../../../../../coalition-game-theory.md), so the [characteristic function of a coalitional game](../../../../../characteristic-function-of-a-coalitional-game.md) must be additive. No [superadditive coalitional game](../../../../../superadditive-coalitional-game.md) or monotonicity assumption is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
