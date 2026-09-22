<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The four row [Gershgorin discs](../../../../gershgorin-disc.md) have centres $9,3,-4,-5$ and radii $1,2,2,1$, respectively. Their real-axis intersections are

$$
[8,10],\qquad[1,5],\qquad[-6,-2],\qquad[-6,-4].
$$

None of the [Gershgorin discs](../../../../gershgorin-disc.md) contains zero, so the [Gershgorin circle theorem](../../../../gershgorin-circle-theorem.md) gives

$$
\boxed{0\notin\operatorname{spec}(A),\quad A\text{ is nonsingular}.}
$$

The discs centred at $9$ and $3$ are each isolated. By [Gershgorin eigenvalue counting](../../../../gershgorin-eigenvalue-counting.md), they contain exactly one [eigenvalue](../../../../eigenvalue.md) apiece, and both [eigenvalues](../../../../eigenvalue.md) are simple. Each must be real: the [characteristic polynomial](../../../../characteristic-polynomial.md) is real, so a nonreal root would bring a distinct conjugate root into the same disc. Denote these [eigenvalues](../../../../eigenvalue.md) by $\beta\in[8,10]$ and $\alpha\in[1,5]$. The remaining two [eigenvalues](../../../../eigenvalue.md) lie in the union of the negative-centred discs.

For the shift $4$, the distances satisfy

$$
|\alpha-4|\leq3,\qquad |\beta-4|\geq4,
\qquad |\gamma-4|\geq6
$$

for either of the other [eigenvalues](../../../../eigenvalue.md) $\gamma$, since its real part is at most $-2$. Thus $\alpha$ is uniquely closest to $4$. Once $4$ is checked not to be an [eigenvalue](../../../../eigenvalue.md), the natural full target-disc [interval enclosure](../../../../interval-enclosure.md) and a conservative asymptotic direction factor are

$$
\boxed{[a,b]=[1,5],\qquad q_4\leq\frac34.}
$$

As always, [inverse iteration](../../../../inverse-iteration.md) requires a nonzero initial target component. The following calculation verifies the shift and gives sharper information.

For the [tridiagonal matrix](../../../../tridiagonal-matrix.md), let $p_j(t)$ be the [determinant](../../../../determinant.md) of the leading $j\times j$ block of $tI-A$. Expansion along the last row gives

$$
\begin{aligned}
p_0(t)&=1,&p_1(t)&=t-9,\\
p_2(t)&=(t-3)(t-9)+1=t^2-12t+28,\\
p_3(t)&=(t+4)p_2(t)-p_1(t)=t^3-8t^2-21t+121,\\
p_4(t)&=(t+5)p_3(t)-p_2(t)
=t^4-3t^3-62t^2+28t+577.
\end{aligned}
$$

In particular, $\det A=577$, $p_4(4)=-239$ and $p_4(5)=-583$. Both shifted [linear systems](../../../../system-of-linear-equations.md) are nonsingular. Further exact evaluations are

$$
\begin{array}{c|rrrrrrrr}
t&-6&-5&-4&-3&3&4&8&9\\\hline
p_4(t)&121&-113&-79&97&103&-239&-607&181.
\end{array}
$$

The [intermediate value theorem](../../../../intermediate-value-theorem.md) gives a real root in each of $(-6,-5)$, $(-4,-3)$, $(3,4)$ and $(8,9)$. As $p_4$ has [polynomial degree](../../../../degree-of-a-polynomial.md) four, these are all its roots and each is simple. In particular, $A$ is a [diagonalizable matrix](../../../../diagonalizable-matrix.md), $\alpha\in(3,4)$ and $\beta\in(8,9)$. The closest competitor to $\alpha$ at the shift $4$ is $\beta$, so this refinement yields

$$
\boxed{\alpha\in[3,4],\qquad q_4=\frac{4-\alpha}{\beta-4}<\frac14.}
$$

For the shift $5$, the original [Gershgorin discs](../../../../gershgorin-disc.md) only give $|\alpha-5|\leq4$ and $|\beta-5|\geq3$; those bounds do not decide which is closer. The refined [interval enclosures](../../../../interval-enclosure.md) do:

$$
1<5-\alpha<2,\qquad3<\beta-5<4,
\qquad|\gamma-5|>8
$$

for the negative [eigenvalues](../../../../eigenvalue.md). Therefore the answer for this particular [matrix](../../../../matrix.md) is yes:

$$
\boxed{\mu=5:\quad\lambda_*=\alpha\in[3,4],\qquad
q_5=\frac{5-\alpha}{\beta-5}<\frac23.}
$$

Both shifts select the same [eigenvector](../../../../eigenvector.md) line and alternate signs because $\alpha<\mu$. The factor bounds concern asymptotic directional convergence, rather than a universal error reduction from the first iterate for a [nonsymmetric matrix](../../../../nonsymmetric-matrix.md). The wider interval $[1,5]$ remains a valid full-disc enclosure for both shifts; $[3,4]$ records the stronger information obtained from the [characteristic polynomial](../../../../characteristic-polynomial.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
