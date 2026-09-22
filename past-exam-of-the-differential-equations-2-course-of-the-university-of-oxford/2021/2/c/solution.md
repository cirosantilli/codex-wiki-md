<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a putative second [Frobenius solution](../../../../frobenius-solution.md) with the smaller [indicial root](../../../../indicial-root.md) $-a$, set $y_-=x^{-a}\sum_{n\geq0}d_nx^n$, with $d_0=1$ and $d_j=0$ for $j<0$. Its [recurrence relation](../../../../recurrence-relation.md) is

$$
\boxed{n(n-2a)d_n=-b\,d_{n-\beta}.}
$$

The [Frobenius case classification](../../../../frobenius-case-classification.md) concerns the gap $2a$ between the [indicial roots](../../../../indicial-root.md). In the course convention, Case IIIa is the obstructed recurrence requiring a [Logarithmic Frobenius solution](../../../../logarithmic-solution-from-a-repeated-frobenius-exponent.md); Case IIIb permits two pure [Frobenius series](../../../../frobenius-solution.md).

If $a>0$ and $2a\notin\mathbb Z$, this is **Case I**: no denominator vanishes. There are two [linearly independent](../../../../linear-independence.md) pure [Frobenius solutions](../../../../frobenius-solution.md), with

$$
y_-(x)=x^{-a}\sum_{k=0}^\infty
\frac{(-b)^kx^{k\beta}}{\prod_{j=1}^k j\beta(j\beta-2a)}.
$$

Their different leading powers establish [linear independence](../../../../linear-independence.md).

If $a=0$, this is **Case II**, with a repeated [indicial root](../../../../indicial-root.md). There is only one pure [Frobenius series](../../../../frobenius-solution.md) with a nonzero leading coefficient. To see the second solution's form, [reduction of order](../../../../reduction-of-order.md) gives

$$
y_2(x)=y_+(x)\int^x\frac{dt}{t\,y_+(t)^2}.
$$

Here $y_+(t)=1+O(t^\beta)$, so the integrand is $t^{-1}+O(t^{\beta-1})$. Consequently

$$
\boxed{y_2(x)=y_+(x)\log x+\text{an analytic power series}.}
$$

The [logarithm](../../../../logarithm.md) has a nonzero coefficient and cannot be removed by adding a multiple of $y_+$.

If $N=2a$ is a positive integer, the only potentially obstructed coefficient is $n=N$. Below that index, $d_n=0$ unless $\beta$ divides $n$. At the exceptional index the equation reads

$$
0=-b\,d_{N-\beta}.
$$

If $N=m\beta$ for some positive integer $m$, all coefficients $d_0,d_\beta,\ldots,d_{(m-1)\beta}$ are nonzero because $b\ne0$. The exceptional equation is inconsistent. This is **Case IIIa**, and the independent second solution has the form

$$
\boxed{y_2=x^{-a}\sum_{n=0}^\infty d_nx^n+K y_+\log x,\qquad K\ne0.}
$$

The [Frobenius resonance for an Euler equation with monomial potential](../../../../frobenius-resonance-for-an-euler-equation-with-monomial-potential.md) explains why divisibility, rather than the integer gap alone, decides this outcome. For example, with $d_0=1$, applying the original [differential operator](../../../../differential-operator.md) to $y_+\log x$ gives $2xy_+'$. Cancellation of the coefficient of $x^a$ requires $K=-bd_{N-\beta}/(2a)\ne0$.

If $\beta$ does not divide $N$, then $d_{N-\beta}=0$; this includes $N<\beta$ through the negative-index convention. The exceptional equation is $0=0$, so $d_N$ is free. This is **Case IIIb**: set $d_N=0$ to select an independent pure [Frobenius series](../../../../frobenius-solution.md) starting with $x^{-a}$. Subsequent coefficients again follow the [recurrence relation](../../../../recurrence-relation.md). Changing $d_N$ simply adds a multiple of $y_+$, the [undetermined coefficient at Frobenius resonance](../../../../undetermined-coefficient-at-frobenius-resonance.md).

The complete answer is therefore

$$
\boxed{\begin{array}{c|c}
\text{parameters}&\text{case}\\\hline
a=0&\mathrm{II}\\
a>0,\quad 2a\notin\mathbb Z&\mathrm{I}\\
2a\in\mathbb N_{>0},\quad 2a/\beta\in\mathbb N_{>0}&\mathrm{IIIa}\\
2a\in\mathbb N_{>0},\quad 2a/\beta\notin\mathbb N_{>0}&\mathrm{IIIb}.
\end{array}}
$$

In particular, for $\beta=1$ every positive integer gap gives Case IIIa. For $\beta=2$, positive integer $a$ gives Case IIIa, while $a=1/2,3/2,5/2,\ldots$ gives Case IIIb; the remaining positive $a$ give Case I. The condition $b\ne0$ matters: at $b=0$ the two [Cauchy-Euler equation](../../../../cauchy-euler-equation.md) powers already give independent solutions whenever $a>0$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the differential equations 2 course of the University of Oxford](../../../split.md)
5. [Differential equations 2 course of the University of Oxford](../../../../differential-equations-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
