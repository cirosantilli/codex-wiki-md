<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume distinct positive separations, and first label them so $A<B$. Let $x=R_0^6$, $a=A^6$ and $b=B^6$. The positive contrast is

$$
\Delta E=E(A)-E(B)=\frac{x}{x+a}-\frac{x}{x+b}
=\frac{x(b-a)}{(x+a)(x+b)}.
$$

Its derivative has a particularly simple sign:

$$
\frac{d\Delta E}{dx}=\frac{(b-a)(ab-x^2)}{(x+a)^2(x+b)^2}.
$$

It is positive below $x=\sqrt{ab}$ and negative above, so this is the global maximum. Both end limits $x\to0$ and $x\to\infty$ give zero contrast. Thus

$$
\boxed{R_{0,\rm opt}=\sqrt{AB},\qquad
\Delta E_{\max}=\frac{B^3-A^3}{B^3+A^3}.}
$$

To recover the printed expression, factor its sixth-power radicand:

$$
\frac{A^6-(AB)^3}{(A/B)^3-1}
=\frac{A^3(A^3-B^3)}{(A^3-B^3)/B^3}=A^3B^3.
$$

Its sixth root is indeed $\sqrt{AB}$. The cancellation requires $A\ne B$. If $A=B$, every choice gives zero contrast and there is no unique optimum; the printed expression then has a removable algebraic $0/0$ without a unique maximization conclusion. For unordered $A,B$, maximize **absolute** contrast and replace the numerator of the maximum by $|B^3-A^3|$. A negative signed difference for $A>B$ is minimized, not maximized, by the same interior point. These qualifications are needed to make the statement precise.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
