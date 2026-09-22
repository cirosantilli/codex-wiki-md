<h1 id="14a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [Möbius transformation of a Papperitz symbol](../../../../../../mobius-transformation-of-a-papperitz-symbol.md) changes the independent variable by a [Möbius transformation](../../../../../../mobius-transformation.md). In particular,

$$
u=\frac{(b-c)(z-a)}{(b-a)(z-c)}
$$

maps $a,b,c$ to $0,1,\infty$, respectively. Because a Möbius map is locally biholomorphic away from its pole, it carries each exponent pair with its singular point and gives

$$
P\left\{
\begin{matrix}
0&1&\infty\\
\alpha&\beta&\gamma\\
\alpha'&\beta'&\gamma'
\end{matrix};u
\right\}.
$$

Now define a [dependent-variable rescaling of a Papperitz symbol](../../../../../../dependent-variable-rescaling-of-a-papperitz-symbol.md) by writing the old dependent variable as

$$
y(u)=u^\alpha(1-u)^\beta v(u),
$$

so that $v=u^{-\alpha}(1-u)^{-\beta}y$. This [dependent-variable rescaling of a Papperitz symbol](../../../../../../dependent-variable-rescaling-of-a-papperitz-symbol.md) subtracts $\alpha$ from both exponents at zero, subtracts $\beta$ from both exponents at one, and adds $\alpha+\beta$ to both exponents at infinity. Hence $v$ has symbol

$$
P\left\{
\begin{matrix}
0&1&\infty\\
0&0&\gamma+\alpha+\beta\\
\alpha'-\alpha&\beta'-\beta&\gamma'+\alpha+\beta
\end{matrix};u
\right\}.
$$

Define

$$
A=\gamma+\alpha+\beta,
\qquad
B=\gamma'+\alpha+\beta,
\qquad
C=1+\alpha-\alpha'.
$$

The Fuchs relation gives $\alpha'-\alpha=1-C$ and $\beta'-\beta=C-A-B$. After renaming $u$ as $z$, the symbol is therefore

$$
\boxed{
P\left\{
\begin{matrix}
0&1&\infty\\
0&0&A\\
1-C&C-A-B&B
\end{matrix};z
\right\}},
$$

which is the [Gauss hypergeometric equation](../../../../../../gauss-hypergeometric-equation.md). Renaming $A,B,C$ as $a,b,c$ gives exactly the displayed symbol in the question.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14A](../../14a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
