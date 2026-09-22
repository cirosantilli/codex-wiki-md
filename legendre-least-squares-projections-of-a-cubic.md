# Legendre least-squares projections of a cubic

↑ **Parent:** [Decoupled coefficients of orthogonal polynomial projections](decoupled-coefficients-of-orthogonal-polynomial-projections.md)

Take the [polynomial](polynomial-split.md) $f(x)=1+x+x^2+x^3$ on $[-1,1]$ with unit weight. Using the four [Legendre polynomials](legendre-polynomial.md) above, direct [integration](integral-split.md) gives

$$
\begin{array}{c|c|c|c|c}
n&h_n&\langle f,P_n\rangle&c_n&c_n^2h_n\\\hline
0&2&8/3&4/3&32/9\\
1&2/3&16/15&8/5&128/75\\
2&2/5&4/15&2/3&8/45\\
3&2/7&4/35&2/5&8/175
\end{array}
$$

For example, $\langle f,P_2\rangle=\tfrac12\int_{-1}^1(3x^4+2x^2-1)\,dx=4/15$: the omitted odd terms have zero [integral](integral-split.md). Dividing by $h_2=2/5$ gives $c_2=2/3$. Substituting all four [coefficients](coefficient.md) proves the exact identity

$$
f=\frac43P_0+\frac85P_1+\frac23P_2+\frac25P_3.
$$

The successive [orthogonal projections](orthogonal-projection.md) onto degrees at most $m$ are therefore

$$
\begin{array}{c|l|c}
m&q_m(x)&E_m=\|f-q_m\|_2^2\\\hline
0&4/3&608/315\\
1&4/3+8x/5&352/1575\\
2&1+8x/5+x^2&8/175\\
3&1+x+x^2+x^3&0
\end{array}
$$

Here $\|g\|_2^2=\int_{-1}^1g(x)^2\,dx$ is the squared [L2 norm](l2-norm.md), without division by the interval length. Each row retains the previous [Legendre polynomial](legendre-polynomial.md) [coefficients](coefficient.md) and appends one new term. The ordinary power [coefficients](coefficient.md) can change: adding $\tfrac23P_2$ changes the constant from $4/3$ to $1$, and adding $\tfrac25P_3$ changes the linear [coefficient](coefficient.md) from $8/5$ to $1$. Independence belongs to the chosen [orthogonal polynomial](orthogonal-polynomial-split.md) coordinates.

<a id="image-nested-legendre-least-squares-projections-of-a-cubic-and-the-exact-squared-residual-contributed-by-each-omitted-mode"></a>
![](legendre-nested-projections-and-residual-budget.png)

**[Figure 2](#image-nested-legendre-least-squares-projections-of-a-cubic-and-the-exact-squared-residual-contributed-by-each-omitted-mode). Nested Legendre least-squares projections of a cubic and the exact squared residual contributed by each omitted mode**.

The full squared [L2 norm](l2-norm.md) is $\|f\|_2^2=192/35$, equal to $32/9+128/75+8/45+8/175$. The residual budgets are the omitted terms:

$$
E_0=\frac{128}{75}+\frac8{45}+\frac8{175}=\frac{608}{315},\qquad E_1=\frac8{45}+\frac8{175}=\frac{352}{1575},\qquad E_2=\frac8{175},\qquad E_3=0.
$$

For a direct check independent of summing the budgets, $f-q_2=x^3-3x/5$, and integrating its square gives $2/7-12/25+6/25=8/175$. This residual is [orthogonal](orthogonal-vectors.md) to $1,x,x^2$, exactly the conditions for the best quadratic [least-squares solution](least-squares-solution-of-a-linear-inverse-problem.md). An [orthogonal projection](orthogonal-projection.md) need not be a [polynomial interpolant](lagrange-polynomial.md): for example, $q_2(1)=18/5$ while $f(1)=4$. The approximation allocates error across the interval according to the chosen [weighted inner product](weighted-inner-product.md).

## ↑ Ancestors (7)

1. [Decoupled coefficients of orthogonal polynomial projections](decoupled-coefficients-of-orthogonal-polynomial-projections.md)
2. [Orthogonal polynomial](orthogonal-polynomial-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Decoupled coefficients of orthogonal polynomial projections](decoupled-coefficients-of-orthogonal-polynomial-projections.md)
