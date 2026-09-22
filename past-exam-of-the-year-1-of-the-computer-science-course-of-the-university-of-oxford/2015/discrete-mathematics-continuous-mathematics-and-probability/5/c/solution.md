<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For positive edge lengths the [volume](../../../../../volume.md) is $V=abc$ and the [surface area](../../../../../surface-area.md) constraint is $2(ab+ac+bc)=S$. Introduce a [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\mu$:

$$
\mathcal L=abc-\mu\bigl(2ab+2ac+2bc-S\bigr).
$$

The [stationary point](../../../../../stationary-point.md) equations are

$$
bc=2\mu(b+c),\qquad ac=2\mu(a+c),\qquad ab=2\mu(a+b).
$$

Multiplying these by $a,b,c$, respectively, and equating their left sides gives $\mu c(a-b)=0$ and $\mu b(a-c)=0$. Because all edge lengths are positive, the equations imply $\mu>0$; hence $a=b=c$. The constraint gives $6a^2=S$.

To establish a global [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md), rather than only a [stationary point](../../../../../stationary-point.md), apply the [arithmetic-geometric mean inequality](../../../../../arithmetic-geometric-mean-inequality.md) to $ab,ac,bc$:

$$
\frac S6=\frac{ab+ac+bc}{3}\ge\bigl((ab)(ac)(bc)\bigr)^{1/3}
=(abc)^{2/3}.
$$

Equality holds exactly when $ab=ac=bc$, or $a=b=c$. Therefore

$$
\boxed{V_{\max}=\left(\frac S6\right)^{3/2},\qquad
 a=b=c=\sqrt{S/6}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
