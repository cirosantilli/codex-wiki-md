<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a line $p(x)=ax+b$, the error $e^x-ax-b$ is strictly convex. Its two endpoint maxima must agree, giving $a=e-1$. Its unique interior minimum is at $c=\log a\in(0,1)$. Equating its magnitude to the endpoint error gives

$$
\boxed{p_1^*(x)=ax+\frac{1+a-a\log a}{2},\qquad
E_1=\frac{1-a+a\log a}{2},\qquad a=e-1.}
$$

The errors at $0,c,1$ are respectively $E_1,-E_1,E_1$. The [equioscillation theorem](../../../../../equioscillation-theorem.md) therefore certifies this [best uniform approximation](../../../../../best-uniform-approximation.md) directly.

For degree above one, subtracting a general [polynomial](../../../../../polynomial-split.md) does not preserve convexity of the error. The required $n+2$ alternating extreme points include additional unknown interior points, and their derivative and equal-height equations form a coupled nonlinear problem. The simple endpoint-and-single-minimum calculation therefore does not extend as a direct higher-degree recipe.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
