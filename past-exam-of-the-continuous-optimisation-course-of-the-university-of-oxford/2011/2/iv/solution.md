<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A sequence is [Q-linearly convergent](../../../../q-linear-convergence.md) to $x^*$ in a specified norm if $\|x_{k+1}-x^*\|\leq q\|x_k-x^*\|$ for all sufficiently large $k$, with some $q<1$. Its asymptotic factor is the limsup of consecutive error ratios.

Put $h=c^{-2}+d^{-2}$, $b_0=c^{-2}-d^{-2}$ and $t=b_0/h$. For an error $e=x-x^*$, an exact first-coordinate step sets $e_1=-te_2$, and an exact second-coordinate step sets $e_2=-te_1$. Once the first coordinate step has occurred, errors consequently alternate between the two lines

$$
e=(-tz,z),\qquad e=(z,-tz).
$$

The next error has its free coordinate multiplied in magnitude by $|t|$, and both lines have the same Euclidean norm factor $\sqrt{1+t^2}$. Therefore, until finite termination,

$$
\boxed{\frac{\|e_{k+1}\|_2}{\|e_k\|_2}
=|t|=\frac{|c^2-d^2|}{c^2+d^2}
=\frac{\kappa_2(H)-1}{\kappa_2(H)+1}<1.}
$$

This is a sharp bound, attained after the first step; the objective errors have factor $t^2$ per step. If $c^2=d^2$, the problem separates and at most two exact steps suffice. When the [condition number](../../../../condition-number.md) is large, the factor approaches one: the iterates zigzag slowly across a narrow tilted valley.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
