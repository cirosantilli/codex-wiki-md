# Diagonal reduction in a two-variable Newton iteration

↑ **Parent:** [Newton's method in optimization](newton-s-method-in-optimization.md)

For $f(x,y)=x^4-4xy+2y^2+4$, the [Newton step](newton-step.md) equations imply $y_{n+1}=x_{n+1}$. Solving the remaining equation gives the displayed scalar recurrence, defined when $3x_n^2\ne1$. Around $(1,1)$ its error factors exactly as

$$
x_{n+1}-1=(x_n-1)^2\frac{2x_n+1}{3x_n^2-1}.
$$

Thus any well-defined sequence converging to $(1,1)$ has [quadratic convergence](quadratic-convergence.md), or reaches that point exactly in finitely many steps. The scalar asymptotic error constant is $3/2$; the [Euclidean norm](euclidean-norm.md) error constant on the diagonal is $3/(2\sqrt2)$. Around $(-1,-1)$, replacing $x$ by $-x$ gives the corresponding conclusion.

## ↑ Ancestors (5)

1. [Newton's method in optimization](newton-s-method-in-optimization.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/continuous-mathematics/6/d/ii/solution.md)
