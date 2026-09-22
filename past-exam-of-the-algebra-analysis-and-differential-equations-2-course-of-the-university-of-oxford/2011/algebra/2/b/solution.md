<h1 id="algebra/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For scalars $\alpha,\beta$ and vectors $v,w,u$, use the adjoint identity and conjugate linearity in the second argument:

$$
\begin{aligned}
\langle u,T^*(\alpha v+\beta w)\rangle
&=\langle Tu,\alpha v+\beta w\rangle\\
&=\overline\alpha\langle Tu,v\rangle+\overline\beta\langle Tu,w\rangle\\
&=\overline\alpha\langle u,T^*v\rangle+\overline\beta\langle u,T^*w\rangle\\
&=\langle u,\alpha T^*v+\beta T^*w\rangle.
\end{aligned}
$$

The difference of the two second-argument vectors is orthogonal to every $u$. Choosing $u$ to be that difference shows its squared [norm](../../../../../norm.md) is zero. Therefore

$$
\boxed{T^*(\alpha v+\beta w)=\alpha T^*v+\beta T^*w.}
$$

The two conjugations are why the adjoint is a linear map, despite the conjugate-linear dependence of the representing functional on its second argument.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Algebra](../../../algebra.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
