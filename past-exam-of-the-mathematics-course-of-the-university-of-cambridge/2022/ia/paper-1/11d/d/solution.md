<h1 id="11d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set

$$
H(x)=(g(b)-g(a))f(x)-(f(b)-f(a))g(x).
$$

Its endpoint values are equal. [Rolle theorem](../../../../../../rolle-theorem.md) therefore supplies $\xi\in(a,b)$ with

$$
(g(b)-g(a))f'(\xi)
=(f(b)-f(a))g'(\xi). \qquad (1)
$$

If $g'(\xi)=0$, then (1) and $g(b)\ne g(a)$ force $f'(\xi)=0$, contrary to the hypothesis. Hence $g'(\xi)\ne0$, and division in (1) gives

$$
\boxed{
\frac{f(b)-f(a)}{g(b)-g(a)}
=\frac{f'(\xi)}{g'(\xi)}}.
$$

The condition is necessary. On $[0,2\pi]$, let

$$
f(x)=\sin x,\qquad
g(x)=\sin x+\frac{x}{4}+\frac{\sin2x}{8}.
$$

Here $g(2\pi)-g(0)=\pi/2$ while $f(2\pi)-f(0)=0$, so the endpoint ratio is zero. But

$$
f'(x)=\cos x,\qquad
g'(x)=\cos x\left(1+\frac12\cos x\right).
$$

Where $g'(x)\ne0$, their ratio is $1/(1+\tfrac12\cos x)$ and is never zero. At the remaining points both derivatives vanish, so the derivative ratio is undefined. Thus the conclusion fails when simultaneous zeros are allowed.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [11D](../../11d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
