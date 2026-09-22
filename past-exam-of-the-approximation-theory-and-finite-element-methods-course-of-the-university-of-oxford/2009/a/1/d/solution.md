<h1 id="a/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [Chebyshev polynomial](../../../../../chebyshev-polynomial.md) identities $T_0=1$, $T_1=x$, and $T_{j+1}=2xT_j-T_{j-1}$. Induction shows that $T_j$ has degree $j$ with leading coefficient $2^{j-1}$ for $j\geq1$. The trigonometric definition also gives

$$
T_n'(\cos\theta)=n\frac{\sin(n\theta)}{\sin\theta}.
$$

Therefore

$$
f_n(x)=\frac{2^{1-n}}n(x^2-1)T_n'(x).
$$

The leading coefficient is $2^{1-n}n^{-1}\cdot n2^{n-1}=1$, and the degree is $n+1$. The endpoints are roots through $x^2-1$; the other $n-1$ points $\cos(s\pi/n)$ are roots through $T_n'$. They are distinct, so this monic polynomial is exactly $\pi_n$.

Differentiating the product $\pi_n(x)=(x-x_s)\pi_{n,s}(x)$ at $x_s$ gives $\pi_n'(x_s)=\pi_{n,s}(x_s)=w_s^{-1}$. For an interior node, differentiate the trigonometric form using $d/dx=-(\sin\theta)^{-1}d/d\theta$:

$$
\pi_n'(\cos\theta)=2^{1-n}
\left[\cot\theta\sin(n\theta)+n\cos(n\theta)\right].
$$

At $\theta_s=s\pi/n$, this is $2^{1-n}n(-1)^s$. At either endpoint, taking the limit makes the two terms equal, doubling the value: $\pi_n'(x_s)=2^{2-n}n(-1)^s$ for $s=0,n$.

After removing the common factor $2^{n-1}/n$, the [barycentric interpolation formula](../../../../../barycentric-interpolation-formula.md) therefore uses

$$
\boxed{w_s=(-1)^s\delta_s,\qquad
\delta_s=1\ (1\leq s<n),\quad \delta_0=\delta_n=\tfrac12.}
$$

These [Chebyshev-Lobatto node](../../../../../chebyshev-lobatto-node.md) weights differ in magnitude by only a factor of two.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
