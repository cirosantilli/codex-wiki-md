# Strictly slack dual constraints force zero primal variables

↑ **Parent:** [Complementary slackness](complementary-slackness.md)

For the primal [linear program](linear-programming-split.md) maximising $c^Tx$ with $Ax\le b$, $x\ge0$, and its [dual linear program](dual-linear-program.md) minimising $b^Ty$ with $A^Ty\ge c$, $y\ge0$, let $x,y$ be optimal. The [complementary slackness](complementary-slackness.md) identity gives $x_j((A^Ty)_j-c_j)=0$. Thus a strict inequality in the $j$th dual constraint forces $x_j=0$. One optimal dual [feasible solution](feasible-point.md) can therefore force zero components in every primal optimum. The same argument with roles reversed says that $y_i>0$ forces the $i$th primal constraint to be an equality.

## ↑ Ancestors (7)

1. [Complementary slackness](complementary-slackness.md)
2. [Linear programming duality](linear-programming-duality.md)
3. [Linear programming](linear-programming-split.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-iv/5/b/ii/solution.md)
