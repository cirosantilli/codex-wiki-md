<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

The [intermediate value theorem](../../../../../intermediate-value-theorem.md) says that a continuous $f:[a,b]\to\mathbb R$ takes every value between $f(a)$ and $f(b)$. For $f(a)<y<f(b)$, the closed sets where $f\leq y$ and $f\geq y$ cannot separate the connected interval; equivalently, taking the supremum of $\{x:f(x)\leq y\}$ and using continuity gives a point with value $y$.

Set $\phi(a)=0$ and $\phi(x)=\sin(1/(x-a))$ for $x>a$. Every interval $[a,b]$ contains a zero $c<b$; continuity on $[c,b]$ makes $\phi$ take every value between $0=\phi(a)$ and $\phi(b)$, yet $\phi$ is discontinuous at $a$.

A monotone [function](../../../../../function-split.md) can be discontinuous only by a jump. If it had a jump at $c$, any number strictly between the left and right [limits](../../../../../limit-of-a-function.md) would lie between $f(a)$ and $f(b)$ but would not be attained, contrary to the hypothesis. Thus it is continuous.

For the last assertion, pass to subsequences with $x_n,y_n$ both within $1/n$ of $a$ and $g(x_n)$ near $l$, $g(y_n)$ near $L$. For $\lambda\in(l,L)$, the intermediate value theorem on the interval joining $x_n$ and $y_n$ gives $z_n$ with $g(z_n)=\lambda$; then $z_n\to a$. The endpoint cases use the original [sequences](../../../../../sequence.md).

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
