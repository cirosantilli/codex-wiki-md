<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Part b(vi) and part c show that $\|T\|_1\leq1$ implies

$$
|\operatorname{tr}(ST)|
\leq\|ST\|_1
\leq\|S\|.
$$

Conversely, choose a unit vector $x$ with $\|Sx\|$ arbitrarily close to $\|S\|$, put $y=Sx/\|Sx\|$, and take $T=x\otimes y$. Part c gives $\|T\|_1=1$ and

$$
\operatorname{tr}(ST)
=\operatorname{tr}(Sx\otimes y)
=\langle Sx,y\rangle
=\|Sx\|.
$$

Taking the supremum proves

$$
\|S\|=\sup_{\|T\|_1\leq1}|\operatorname{tr}(ST)|.
$$

Thus $S\mapsto[T\mapsto\operatorname{tr}(ST)]$ is an isometric embedding $\mathcal S_\infty\to\mathcal S_1^*$.

Suppose finite-rank operators are dense in $\mathcal S_1$ and let $L\in\mathcal S_1^*$. The sesquilinear form

$$
b(x,y)=L(x\otimes y)
$$

satisfies $|b(x,y)|\leq\|L\|\|x\|\|y\|$. The [Riesz representation theorem](../../../../../../riesz-representation-theorem.md) gives $S\in\mathcal S_\infty$ with $b(x,y)=\langle Sx,y\rangle$. Hence $L(x\otimes y)=\operatorname{tr}(S(x\otimes y))$, and linearity gives equality on every finite-rank operator. Density and continuity extend it to every $T\in\mathcal S_1$, proving surjectivity.

Conversely, if finite-rank operators were not dense, the [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) would give a nonzero $L\in\mathcal S_1^*$ vanishing on their closure. Surjectivity would represent it by some $S$, but then

$$
0=L(x\otimes y)=\langle Sx,y\rangle
$$

for all $x,y$, forcing $S=0$ and $L=0$, a contradiction. This proves the stated [trace duality](../../../../../../trace-duality.md) criterion.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
