<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the convention $0\log_20=0$. On the positive support of $p$, the given logarithm inequality gives

$$
D(p,q)=-\sum_{p_r>0}p_r\log_2(q_r/p_r)\ge c\sum_{p_r>0}(p_r-q_r)\ge0.
$$

The logarithm is strictly concave, so its supporting line at one has equality only there. More explicitly, the given global bound forces $c=1/\log_e2$ by differentiation at one, and $x-1-\log_ex$ vanishes only at one. Equality above therefore requires $p_r=q_r$ on the positive support, and no mass of $q$ outside it. Thus **equality holds exactly when $p=q$**.

For the uniform distribution $q_r=1/n$, the divergence is $D(p,q)=\log_2n-H(p)$. Its nonnegativity gives $\boxed{H(p)\le\log_2n}$, with equality precisely for the uniform law.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
