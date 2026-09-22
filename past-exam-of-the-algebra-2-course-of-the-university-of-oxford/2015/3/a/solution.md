<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonzero [polynomial](../../../../polynomial-split.md) $f=\sum_i a_it^i\in\mathbb Z[t]$, its [polynomial content](../../../../polynomial-content.md) is the positive [greatest common divisor](../../../../greatest-common-divisor.md) of its coefficients:

$$
c(f)=\gcd(a_0,a_1,\ldots)>0.
$$

For nonzero $g\in\mathbb Q[t]$, choose a positive [integer](../../../../integer-split.md) $n$ with $ng\in\mathbb Z[t]$ and define its [rational polynomial content](../../../../rational-polynomial-content.md) by

$$
\boxed{c(g)=\frac{c(ng)}n.}
$$

To check independence of the denominator, write $g=f/n=h/m$ with $f,h\in\mathbb Z[t]$ and $n,m>0$. Then $mf=nh$, while multiplication of all coefficients by a positive [integer](../../../../integer-split.md) gives

$$
mc(f)=c(mf)=c(nh)=nc(h).
$$

Dividing by $mn$ proves $c(f)/n=c(h)/m$, as required.

For multiplication, write $g_i=f_i/n_i$. The integer-coefficient content identity permitted in the source gives

$$
\begin{aligned}
c(g_1g_2)
&=\frac{c(f_1f_2)}{n_1n_2}
=\frac{c(f_1)c(f_2)}{n_1n_2}\\
&=c(g_1)c(g_2).
\end{aligned}
$$

Thus

$$
\boxed{c(g_1g_2)=c(g_1)c(g_2).}
$$

We will also use the normalization $g/c(g)\in\mathbb Z[t]$, with content one: if $g=f/n$, then $g/c(g)=f/c(f)$. It is a [primitive polynomial](../../../../primitive-polynomial.md). For a nonzero rational constant $r$, the same definition gives $c(r)=|r|$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the algebra 2 course of the University of Oxford](../../../split.md)
5. [Algebra 2 course of the University of Oxford](../../../../algebra-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
