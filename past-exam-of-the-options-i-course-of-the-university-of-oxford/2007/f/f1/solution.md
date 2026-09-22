<h1 id="f/f1/solution">Solution</h1>

↑ **Parent:** [F1](../f1.md)

The [implicit function theorem](../../../../implicit-function-theorem.md) applies when $D_2F(a,b)\ne0$. After shrinking the neighbourhood, this partial derivative stays nonzero along the implicit [graph](../../../../graph-split.md). Differentiating its defining identity gives

$$
f'(x)=-\frac{D_1F(x,f(x))}{D_2F(x,f(x))}.
$$

For the specified smooth function, $F_x=y+\cos(x+y)$ and $F_y=x+\cos(x+y)$, so both equal one at zero. In particular the theorem applies and $f'(0)=-1$. Differentiate the identity a second time:

$$
F_{xx}+2F_{xy}f'+F_{yy}(f')^2+F_yf''=0.
$$

At zero, $F_{xx}=F_{yy}=0$ and $F_{xy}=1$. Therefore

$$
\boxed{f'(0)=-1,\qquad f''(0)=2}.
$$

## ↑ Ancestors (12)

1. [F1](../f1.md)
2. [F](../../f.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
