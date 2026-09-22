<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

[Gradient descent](../../../../../gradient-descent.md) is $x_{t+1}=x_t-\eta\nabla f(x_t)$. Integrating the Hessian along a segment gives the descent lemma. Applying it to the hinted $z$ and convexity yields cocoercivity: $(\nabla f(x)-\nabla f(y))^T(x-y)\ge\|\nabla f(x)-\nabla f(y)\|^2/\beta$. Apply this to $\phi=f-\alpha\|x\|^2/2$, whose Hessian lies between $0$ and $(\beta-\alpha)I$, and rearrange to obtain the displayed strengthened inequality. With $y=x^*$, $\nabla f(x^*)=0$, and $\eta=2/(\alpha+\beta)$, expansion of the squared update gives contraction factor $((\beta-\alpha)/(\beta+\alpha))^2$ per step and the stated bound.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
