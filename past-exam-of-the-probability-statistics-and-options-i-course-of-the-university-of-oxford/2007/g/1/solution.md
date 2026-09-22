<h1 id="g/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $\eta$ be a smooth [variation](../../../../variation.md) with $\eta=\eta'=0$ at both endpoints, and consider $y_\epsilon=y+\epsilon\eta$. [stationary point](../../../../stationary-point.md) gives the [first variation](../../../../first-variation.md)

$$
0=\left.\frac d{d\epsilon}J[y_\epsilon]\right|_{\epsilon=0}
=\int_{x_1}^{x_2}
\left(F_y\eta+F_{y'}\eta'+F_{y''}\eta''\right)dx.
$$

Integrate the middle term once by parts and the last term twice. All boundary terms vanish because both $\eta$ and $\eta'$ vanish there. Assuming the derivatives needed for the classical formula, the given [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) yields

$$
\boxed{F_y-\frac d{dx}F_{y'}+
\frac{d^2}{dx^2}F_{y''}=0.}
$$

Without assuming those classical derivatives initially, the same calculation with compactly supported variations states this equation weakly; sufficient regularity then gives the classical equation.

For the specific integrand, $F_y=-2y$, $F_{y'}=0$, $F_{y''}=2y''$, so the equation is $y^{(4)}-y=0$. Its [weak solutions](../../../../weak-solution.md) here are smooth, and its general classical solution is

$$
y=A\cos x+B\sin x+C\cosh x+D\sinh x.
$$

Put $\ell=\pi/2$, $c=\cosh\ell$, $s=\sinh\ell$. The conditions at zero give $C=-A$ and $D=1-B$. Those at $\ell$ give

$$
B-Ac+(1-B)s=0,\qquad
-A-As+(1-B)c=0.
$$

Using $c^2-s^2=1$, solve to obtain $A=c/2$, $B=(1-s)/2$, $C=-c/2$, $D=(1+s)/2$. Thus an [extremal](../../../../extremal.md) is

$$
\boxed{y(x)=\frac12\left[
c(\cos x-\cosh x)+(1-s)\sin x+(1+s)\sinh x
\right].}
$$

Substitution checks all four boundary values. The additive term $x^2$ in the integrand contributes no [variation](../../../../variation.md) in $y$, so it does not alter this equation.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [G](../../g.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
