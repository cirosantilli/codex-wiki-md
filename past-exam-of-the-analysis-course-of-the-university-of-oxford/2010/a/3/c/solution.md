<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [multiplication operator](../../../../../multiplication-operator.md), $\|Tf\|_\infty\leq\|g\|_\infty\|f\|_\infty=\|f\|_\infty$. Taking $f=1$ gives equality, so $\|T\|=1$.

An [eigenfunction](../../../../../eigenfunction.md) obeys $(g(t)-\lambda)f(t)=0$ at every $t$. If $\lambda\in[0,1)$, its level set is the single point $t=\lambda$, and a [continuous function](../../../../../continuous-function.md) supported at a single point is zero. If $\lambda\notin[0,1]$, that level set is empty. For $\lambda=1$, every [continuous function](../../../../../continuous-function.md) vanishing on $[0,1]$ is an [eigenfunction](../../../../../eigenfunction.md), and nonzero examples exist, such as $f(t)=\max\{t-1,0\}$. Thus $\sigma_p(T)=\{1\}$.

If $\lambda\notin[0,1]$, multiplication by $(g-\lambda)^{-1}$ is a bounded inverse of $T-\lambda I$. If $\lambda\in[0,1]$, choose $t_0$ with $g(t_0)=\lambda$. Every function in the range of $T-\lambda I$ vanishes at $t_0$, so the range omits the constant function one. Hence it is not onto. Therefore

$$
\boxed{\|T\|=1,\qquad\sigma_p(T)=\{1\},\qquad\sigma(T)=[0,1].}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
