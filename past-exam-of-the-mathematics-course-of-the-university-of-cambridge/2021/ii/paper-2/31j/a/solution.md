<h1 id="31j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [convex function](../../../../../../convex-function.md) $f$, its [subdifferential](../../../../../../subdifferential.md) is

$$
\partial f(x)=\{g:f(y)\geq f(x)+g^T(y-x)\text{ for every }y\}.
$$

For $f(x)=\gamma|x|$,

$$
\partial f(x)=
\begin{cases}
\{\gamma\},&x>0,\\
[-\gamma,\gamma],&x=0,\\
\{-\gamma\},&x<0.
\end{cases}
$$

The defining inequality shows directly that $0\in\partial f(x)$ exactly when $x$ is a global minimizer.

Strict convexity means

$$
f(\lambda x+(1-\lambda)y)<\lambda f(x)+(1-\lambda)f(y)
$$

for distinct $x,y$ and $0<\lambda<1$. Two distinct minimizers would make the midpoint have a strictly smaller value, so a minimizer is unique.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31J](../../31j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
