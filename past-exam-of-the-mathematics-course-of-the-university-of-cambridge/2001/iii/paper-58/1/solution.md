<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [cubic spline](../../../../../cubic-spline.md) is even, so the symmetry of the normalized [B-splines](../../../../../b-spline.md) gives $N_{j,4}(-x)=N_{6-j,4}(x)$. It therefore suffices to extract three [coefficients](../../../../../coefficient.md). The two [polynomial](../../../../../polynomial-split.md) pieces join with matching values and first two [derivatives](../../../../../derivative.md) at zero, so the function belongs to the stated [cubic spline](../../../../../cubic-spline.md) space. At zero its right-hand [derivatives](../../../../../derivative.md) are

$$
f(0)=1,\qquad f'(0)=0,\qquad f''(0)=-27,\qquad f'''(0+)=81.
$$

Use the supplied [De Boor–Fix spline coefficient functional](../../../../../de-boor-fix-spline-coefficient-functional.md) with the unnormalized knot [polynomial](../../../../../polynomial-split.md) $\psi_j(x)=\prod_{r=j+1}^{j+3}(t_r-x)$. In this sign convention the [coefficient](../../../../../coefficient.md) is

$$
c_j=\frac{\psi_jf'''-\psi_j'f''+\psi_j''f'-\psi_j'''f}{6}.
$$

For $j=1$, $\psi_1=(-1-x)^3$. Taking the right-hand limit at $-1$ kills the first three terms and gives $c_1=f(-1)=1$. For the next two [coefficients](../../../../../coefficient.md) take the right-hand limit at zero. Their knot [polynomials](../../../../../polynomial-split.md) and [derivatives](../../../../../derivative.md) there are

$$
\begin{aligned}
\psi_2(x)&=-x(1+x)^2,&(\psi_2,\psi_2',\psi_2'',\psi_2''')(0)&=(0,-1,-4,-6),\\
\psi_3(x)&=x-x^3,&(\psi_3,\psi_3',\psi_3'',\psi_3''')(0)&=(0,1,0,-6).
\end{aligned}
$$

Consequently $c_2=(-27+6)/6=-7/2$ and $c_3=(27+6)/6=11/2$. Although the third [derivative](../../../../../derivative.md) jumps at zero, its multiplier $\psi_j(0)$ vanishes for these two [functionals](../../../../../functional.md); taking either one-sided limit gives the same [coefficients](../../../../../coefficient.md). Symmetry gives $c_4=c_2$ and $c_5=c_1$. Thus

$$
\boxed{(c_1,c_2,c_3,c_4,c_5)=(1,-7/2,11/2,-7/2,1).}
$$

For a normalized [B-spline](../../../../../b-spline.md) [basis](../../../../../basis.md), define the synthesis [linear map](../../../../../linear-map.md) $Tc=\sum_jc_jN_{j,4}$ from the maximum [coefficient](../../../../../coefficient.md) [norm](../../../../../norm.md) into the [spline](../../../../../spline-mathematics.md) space with its [supremum norm](../../../../../supremum-norm.md). Nonnegativity and partition of unity give $\|T\|=1$, including equality on the all-ones [vector](../../../../../vector.md). The [coefficient condition number of a normalized B-spline basis](../../../../../coefficient-condition-number-of-a-normalized-b-spline-basis.md) is

$$
\kappa(\mathcal S)=\|T\|\|T^{-1}\|=\sup_{0\ne s\in\mathcal S}\frac{\|c(s)\|_{\ell^\infty}}{\|s\|_\infty}.
$$

On $[0,1]$, $f'(x)=(27/2)x(3x-2)$. The only interior extremum is at $2/3$, where $f=-1$; at zero and one, $f=1$. Reflection therefore gives $\|f\|_\infty=1$. Its largest absolute [coefficient](../../../../../coefficient.md) is $11/2$, proving

$$
\boxed{\kappa(\mathcal S)\ge\frac{11}{2}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
