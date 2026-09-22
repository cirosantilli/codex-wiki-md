<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a [flex](../../../../../../inflection-point-of-an-algebraic-plane-curve.md) as $O=[0:1:0]$, with [tangent line](../../../../../../tangent-line.md) $Z=0$. The [flex coordinates for a smooth plane cubic](../../../../../../flex-coordinates-for-a-smooth-plane-cubic.md) give

$$
F=aX^3+bY^2Z+cXYZ+dX^2Z+eYZ^2+fXZ^2+gZ^3,
\qquad ab\ne0.
$$

The coefficient $a$ is nonzero because $Z=0$ is not a component, and $b\ne0$ expresses smoothness at $O$. Since the [field characteristic](../../../../../../characteristic-of-a-field.md) is not two, the projective linear change

$$
Y'=Y+\frac{cX+eZ}{2b}
$$

completes the square. The equation becomes $Y'^2Z=P_3(X,Z)$ after dividing by a nonzero constant, where $P_3$ is a degree-three [homogeneous polynomial](../../../../../../homogeneous-polynomial.md) with nonzero $X^3$ coefficient.

On $Z=1$, the [polynomial](../../../../../../polynomial-split.md) $P_3(x,1)$ has three distinct roots $r_1,r_2,r_3$ in the [algebraically closed field](../../../../../../algebraically-closed-field.md). A repeated root $r$ would make $(r,0)$ a [singular point](../../../../../../singular-point-of-an-algebraic-variety.md) of $y'^2=P_3(x,1)$, since both first partial derivatives vanish there. Put

$$
x'=\frac{x-r_1}{r_2-r_1},\qquad
\lambda=\frac{r_3-r_1}{r_2-r_1}.
$$

A further nonzero scaling of $y'$ absorbs the leading coefficient and $(r_2-r_1)^3$; the required square root exists in the [algebraically closed field](../../../../../../algebraically-closed-field.md). These are projective linear changes of the original coordinates. Renaming the new coordinates gives the [Legendre form of an elliptic curve](../../../../../../legendre-form-of-an-elliptic-curve.md)

$$
\boxed{y^2=x(x-1)(x-\lambda),\qquad\lambda\notin\{0,1\}.}
$$

Its projective completion is $Y^2Z=X(X-Z)(X-\lambda Z)$, with the chosen [flex](../../../../../../inflection-point-of-an-algebraic-plane-curve.md) at infinity.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
