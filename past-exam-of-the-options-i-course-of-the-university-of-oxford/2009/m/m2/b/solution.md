<h1 id="m/m2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $u_n=\mathbb P(X_n=1\mid X_0=1)$. Conditioning on $X_n$ gives

$$
u_{n+1}=(1-a)u_n+b(1-u_n)=b+(1-a-b)u_n,\qquad u_0=1.
$$

The fixed value is $b/(a+b)$. Subtracting it and iterating the scalar recurrence yields

$$
\boxed{u_n=\frac b{a+b}+\frac a{a+b}(1-a-b)^n},\qquad n\geq0.
$$

The formula includes $n=0$. If $a+b=1$, its value at $n=0$ is interpreted directly as $u_0=1$, while $u_n=b$ for all $n\geq1$. Since $|1-a-b|<1$, the limiting probability is $b/(a+b)$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [M2](../../m2.md)
3. [M](../../../m.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
