<h1 id="f/f2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the scalar function $H(s)=\langle f(x+s(y-x)),z\rangle$ on $[0,1]$. It is [continuous](../../../../../continuous-function.md) there and [differentiable](../../../../../differentiable-function.md) inside, with [derivative](../../../../../derivative.md) $\langle df(x+s(y-x))(y-x),z\rangle$ by the chain rule. The one-dimensional [mean value theorem](../../../../../mean-value-theorem.md) gives $H(1)-H(0)=H'(\theta)$ for some $0<\theta<1$, proving the displayed vector-paired version. No claim of a single intermediate point giving a vector equality without pairing is required.

For the final assertion, use the scalar [mean value theorem](../../../../../mean-value-theorem.md) directly on $s\mapsto g(sh)$: it is [continuous](../../../../../continuous-function.md) at $s=0$ and [differentiable](../../../../../differentiable-function.md) for $s>0$. Thus

$$
g(h)-g(0)=\nabla g(\theta_hh)\cdot h
$$

for some $0<\theta_h<1$. The assumed limits of all partial [derivatives](../../../../../derivative.md) imply $\|\nabla g(x)\|\to0$ as $x\to0$, $x\ne0$. Consequently $|g(h)-g(0)|/\|h\|\le\|\nabla g(\theta_hh)\|\to0$. Hence $\boxed{dg(0)=0}$ and $g$ is [differentiable](../../../../../differentiable-function.md) there. This argument uses only [differentiability](../../../../../differentiability.md) on the interior of the line segment, so it does not assume the conclusion at its endpoint.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [F2](../../f2.md)
3. [F](../../../f.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
