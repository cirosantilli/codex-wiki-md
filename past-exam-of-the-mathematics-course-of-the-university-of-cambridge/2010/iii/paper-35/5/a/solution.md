<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

It is useful to prove the general [core of the miners game](../../../../../../core-of-the-miners-game.md) calculation when $r$ miners carry one unit: $v(S)=\lfloor|S|/r\rfloor$, with $r\geq2$. Individual rationality gives $x_i\geq0$, and efficiency gives $\sum_i x_i=q:=\lfloor n/r\rfloor$.

If $n<r$, the grand coalition value is zero and the only core allocation is zero. If $n\geq r$, every $r$-person coalition must receive at least one. Sum these inequalities over all $\binom nr$ such coalitions. Each player appears $\binom{n-1}{r-1}$ times, so

$$
\binom{n-1}{r-1}q\geq\binom nr,\qquad \frac{rq}{n}\geq1.
$$

If $r$ does not divide $n$, then $rq<n$, a contradiction. Thus the [core of a cooperative game](../../../../../../core-game-theory.md) is empty in these cases.

If $n=r$, every proper coalition has value zero. The core is exactly the simplex of nonnegative allocations with total one. If $n$ is a multiple of $r$ with $n\geq2r$, the averaged inequality is equality. Since each $r$-person coalition sum is at least one, every such sum equals one. For any two players $i,j$, choose $r-1$ other players and compare the two resulting $r$-person coalition sums. They imply $x_i=x_j$. Hence $x_i=1/r$ for all players. This vector belongs to the core because $|S|/r\geq\lfloor|S|/r\rfloor$ for every coalition.

For two miners per lump, therefore,

$$
\boxed{C_2(n)=\begin{cases}
\{(0)\},&n=1,\\
\{(x_1,x_2):x_i\geq0,\ x_1+x_2=1\},&n=2,\\
\{(1/2,\ldots,1/2)\},&n\geq4\text{ even},\\
\varnothing,&n\geq3\text{ odd}.
\end{cases}}
$$

In particular the even case has a small-group exception at $n=2$.

For three miners per lump, the same proof gives

$$
\boxed{C_3(n)=\begin{cases}
\{(0,\ldots,0)\},&n=1,2,\\
\{x\in\mathbb R_+^3:x_1+x_2+x_3=1\},&n=3,\\
\{(1/3,\ldots,1/3)\},&n\geq6,\ 3\mid n,\\
\varnothing,&n\geq4,\ 3\nmid n.
\end{cases}}
$$

Thus divisibility controls the existence of a stable allocation once enough miners are present, while exactly one possible lump leaves freedom to divide its value.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
