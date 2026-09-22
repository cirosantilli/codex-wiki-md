<h1 id="f/f2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x\ne y$, apply the scalar [mean value theorem](../../../../../mean-value-theorem.md) to $h(t)=\langle f(x+t(y-x)),z\rangle$ on $[0,1]$. It is [continuous](../../../../../continuous-function.md) on the closed interval and differentiable inside by the stated segment and regularity assumptions. The [chain rule](../../../../../chain-rule.md) gives

$$
h'(t)=\langle Df(x+t(y-x))(y-x),z\rangle.
$$

Thus $h(1)-h(0)=h'(\theta)$ for some $\theta\in(0,1)$, precisely the asserted identity. If $x=y$, both sides are zero when the zero-direction derivative is naturally taken as $Df(x)0$.

For the final claim, all partial derivatives tending to zero imply $\|\nabla g(x)\|\to0$ away from the origin. For a nonzero small vector $h$, the one-variable [function](../../../../../function-split.md) $t\mapsto g(th)$ is [continuous](../../../../../continuous-function.md) on $[0,1]$ by [continuity](../../../../../continuous-function.md) at zero and differentiable on $(0,1)$. Therefore

$$
g(h)-g(0)=\nabla g(\theta h)\cdot h
$$

for some $\theta\in(0,1)$. For any $\varepsilon>0$, if $\|h\|$ is sufficiently small, the entire punctured segment has [gradient](../../../../../gradient.md) [norm](../../../../../norm.md) below $\varepsilon$. Hence $|g(h)-g(0)|\leq\varepsilon\|h\|$, proving

$$
\boxed{Dg(0)=0}.
$$

This argument does not presuppose [differentiability](../../../../../differentiability.md) at the origin.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [F2](../../f2.md)
3. [F](../../../f.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
