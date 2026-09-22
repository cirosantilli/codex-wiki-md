<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\theta=e^\beta$ for the group-1 to group-0 hazard ratio. At $t_1$, all four subjects are at risk, so subject 1 contributes $1/(2+2\theta)$. At $t_2$, subjects 2, 3, and 4 are at risk, so subject 2 contributes $\theta/(1+2\theta)$.

If $t_2<c<t_4$, subject 3 leaves before $t_4$ and subject 4, if it fails, is alone in its risk set. Hence

$$
L_p(\theta)=\frac1{2+2\theta}\frac{\theta}{1+2\theta},
$$

independently of $k$. Its log derivative vanishes when $1-2\theta^2=0$, giving

$$
\widehat\theta=\frac1{\sqrt2}.
$$

If $c=t_4$, subject 3 remains in the risk set at a failure of subject 4. Therefore

$$
L_p(\theta)=\frac1{2+2\theta}\frac{\theta}{1+2\theta}
\left(\frac1{1+\theta}\right)^k.
$$

For $k=0$, $\widehat\theta=1/\sqrt2$. For $k=1$, the score equation is $1-\theta-4\theta^2=0$, so

$$
\widehat\theta=\frac{\sqrt{17}-1}{8}\simeq0.39.
$$

**Thus $\widehat\theta$ is constant at $1/\sqrt2$ for $t_2\leq c<t_4$. At $c=t_4$ it remains there when $k=0$ and drops to approximately $0.39$ when $k=1$, because only then does the censoring time change an event's risk set.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
