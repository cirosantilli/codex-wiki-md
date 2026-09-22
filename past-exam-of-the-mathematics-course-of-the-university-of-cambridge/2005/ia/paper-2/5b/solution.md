<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

The [characteristic equation of a linear recurrence](../../../../../characteristic-equation-of-a-linear-recurrence.md) is

$$
r^2-2\cos\theta\,r+1=0,
\qquad r=e^{\pm i\theta}.
$$

For $0<\theta<\pi$, these [characteristic roots](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) are distinct. Two real solutions of the [second-order difference equation](../../../../../second-order-difference-equation.md) are $\cos(n\theta)$ and $\sin(n\theta)$. Their values at $n=0,1$ form a [matrix](../../../../../matrix.md) with [determinant](../../../../../determinant.md) $\sin\theta\ne0$, proving [linear independence](../../../../../linear-independence.md). Consequently they span the two-dimensional [vector space](../../../../../vector-space-split.md) of recurrence solutions.

At $\theta=0$ the two roots coalesce at one. The [linear recurrence](../../../../../linear-recurrence-relation.md) becomes $X_{n+2}-X_{n+1}=X_{n+1}-X_n$, so its successive differences are constant. A [basis](../../../../../basis.md) is therefore **$1,n$**, and every solution is $A+Bn$.

For the specified [initial conditions](../../../../../initial-condition.md), the zero-angle solution is $X_n(0)=n$. For nonzero angle, it is convenient to center the [basis](../../../../../basis.md) at $n=1$:

$$
\boxed{X_n(\theta)=\cos((n-1)\theta)
+\frac{2-\cos\theta}{\sin\theta}\sin((n-1)\theta),\qquad 0<\theta<\pi.}
$$

This gives $X_1=1$ and $X_2=\cos\theta+2-\cos\theta=2$, and each summand obeys the [linear recurrence](../../../../../linear-recurrence-relation.md). For every fixed integer $n\geq1$, the elementary [limit](../../../../../limit-of-a-function.md) $\sin z/z\to1$ gives

$$
\frac{\sin((n-1)\theta)}{\sin\theta}\longrightarrow n-1,
\qquad \boxed{X_n(\theta)\longrightarrow1+(n-1)=n=X_n(0).}
$$

The convergence here is for fixed $n$; it does not assert uniform convergence over all indices.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
