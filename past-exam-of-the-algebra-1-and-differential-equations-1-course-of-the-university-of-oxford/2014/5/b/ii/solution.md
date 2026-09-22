<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use an exponential perturbation whose image under $L$ is strictly positive everywhere. The coefficient $r$ is bounded on the closed disk; put $R=\max_{\overline D}|r|$ and choose $k>R$, $k>0$. For $v(x,y)=e^{kx}$,

$$
Lv=(k^2+kr(x,y))e^{kx}\geq k(k-R)e^{kx}>0.
$$

Consequently $u_\epsilon=u+\epsilon v$ satisfies $Lu_\epsilon=f+\epsilon Lv>0$. Part (i) applies, so for every $z\in\overline D$,

$$
u(z)+\epsilon v(z)\leq\max_{\partial D}(u+\epsilon v)
\leq\max_{\partial D}u+\epsilon e^k.
$$

Letting $\epsilon\downarrow0$ gives

$$
\boxed{u(z)\leq\max_{\partial D}u.}
$$

Thus **the maximum is attained on the boundary also when $f\geq0$**. This is the [exponential perturbation proof of the weak maximum principle with drift](../../../../../exponential-perturbation-proof-of-the-weak-maximum-principle-with-drift.md). It does not require differentiating the continuous coefficients $r,s$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
