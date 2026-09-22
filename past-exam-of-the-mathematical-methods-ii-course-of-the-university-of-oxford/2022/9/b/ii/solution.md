<h1 id="9/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $F'=f$ and $G'=g$ on the relevant intervals. The [chain rule](../../../../../chain-rule.md) gives

$$
d\{F(xy)+G(y/x)\}
=\left[yf(xy)-\frac y{x^2}g(y/x)\right]dx
+\left[xf(xy)+\frac1xg(y/x)\right]dy.
$$

Thus the one-form is explicitly an [exact differential](../../../../../exact-differential.md). Fixing its potential to vanish at $(1,1)$ determines it uniquely on the connected domain:

$$
\boxed{\phi(x,y)=\int_1^{xy}f(s)\,ds+\int_1^{y/x}g(t)\,dt.}
$$

Continuity of $f,g$ on the integration ranges suffices. For arbitrary smooth data defined throughout $x>0$, that half-plane also supplies the simply connected domain in the previous argument.

For the specialization $f(s)=s^{-2}$, the potential based at $(1,1)$ is defined in the positive quadrant; it cannot be continued through $xy=0$ using this formula. Taking $a,b>0$ keeps both endpoints in that component. Their ratios $y/x$ are both $b/a$, so the $G$ term cancels and

$$
\boxed{\phi(ab,b^2)-\phi(a,b)=\int_{ab}^{ab^3}s^{-2}\,ds
=\frac{b^2-1}{ab^3}.}
$$

No condition on $g$ beyond existence on the traversed ratios enters this difference.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the mathematical methods II course of the University of Oxford](../../../../split.md)
6. [Mathematical methods II course of the University of Oxford](../../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
