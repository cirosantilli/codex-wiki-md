<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [entropy summand](../../../../entropy-summand.md) $f(x)=-x\log x$, differentiation on $(0,1)$ gives

$$
f'(x)=-\frac{\ln x+1}{\ln2},\qquad f''(x)=-\frac1{x\ln2}<0.
$$

Since $f(x)\to0$ as $x\downarrow0$, its continuous extension to $[0,1]$ is a [concave function](../../../../concave-function.md).

Fix $0<v<1$ and define the increment $D_v(t)=f(t+v)-f(t)$ on $[0,1-v]$. In its interior,

$$
D_v'(t)=f'(t+v)-f'(t)=-\log\frac{t+v}{t}<0.
$$

Thus the increment is decreasing, and its endpoint values are $D_v(0)=f(v)$ and $D_v(1-v)=-f(1-v)$. Therefore

$$
-f(1-v)\leq f(t+v)-f(t)\leq f(v),
\qquad
\boxed{|f(t+v)-f(t)|\leq\max\{f(v),f(1-v)\}.}
$$

The cases $v=0,1$ follow directly from the endpoint values.

To obtain the sharper half-interval bound, put $G(v)=f(v)-f(1-v)$. It has $G(0)=G(1/2)=0$, while

$$
G''(v)=\frac{2v-1}{v(1-v)\ln2}\leq0\qquad(0<v\leq1/2).
$$

Hence $G$ is a [concave function](../../../../concave-function.md) on $[0,1/2]$ and lies above the chord joining its zero endpoints. Thus $f(v)\geq f(1-v)$ there, proving

$$
\boxed{|f(t+v)-f(t)|\leq f(v)\qquad(0\leq v\leq1/2).}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
