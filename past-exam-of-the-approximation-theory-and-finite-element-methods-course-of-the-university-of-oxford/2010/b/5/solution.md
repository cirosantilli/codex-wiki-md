<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Take the affine trial space $V_1=\{v\in H^1(a,b):v(a)=1\}$ and the test space $V_0=\{v\in H^1(a,b):v(a)=0\}$. Multiplication by $v\in V_0$ and [integration by parts](../../../../integration-by-parts.md) incorporate the right [Neumann boundary condition](../../../../neumann-boundary-condition.md) as a load:

$$
\boxed{u\in V_1,\qquad\int_a^bu'v'\,dx=\int_a^bfv\,dx+2v(b)\quad(v\in V_0).}
$$

For the continuous piecewise-quadratic trial space, impose the left value exactly and use the same equation for every piecewise-quadratic test function vanishing at $a$. With a [basis](../../../../basis.md) $(\psi_j)$ of that test space and $u_h=1+\sum_jc_j\psi_j$, the [finite element](../../../../finite-element.md) equations are

$$
\boxed{\sum_j\left(\int_a^b\psi_j'\psi_i'\,dx\right)c_j=\int_a^bf\psi_i\,dx+2\psi_i(b).}
$$

The [Endpoint Poincaré inequality](../../../../endpoint-poincare-inequality.md), reflected about the interval midpoint, makes the derivative norm a norm on $V_0$. [Galerkin orthogonality](../../../../galerkin-orthogonality.md) then gives the exact best-approximation identity: for every admissible $v_h$,

$$
\|u'-v_h'\|_2^2=\|u'-u_h'\|_2^2+\|u_h'-v_h'\|_2^2.
$$

Therefore **$u_h$ minimizes the derivative error over all admissible piecewise-quadratic functions**.

To prove the requested error bound, assume $f\in H^1(a,b)$. Then $u\in H^3(a,b)$ and $u'''=-f'$. We need an elementary [Poincare-Wirtinger inequality](../../../../poincare-wirtinger-inequality.md) on each element $I$ of length $h_I$: if $w\in H^1(I)$ has mean zero, its continuous representative has a zero somewhere, and the [fundamental theorem of calculus](../../../../fundamental-theorem-of-calculus.md) and [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) give $\|w\|_{L^2(I)}\leq h_I\|w'\|_{L^2(I)}$.

Choose an affine function $q_I$ whose slope is the average of $u''$ on $I$ and whose average equals the average of $u'$. Then $w=u'-q_I$ and $w'=u''-q_I'$ both have mean zero. Applying the just-proved bound twice yields

$$
\|u'-q_I\|_{L^2(I)}\leq h_I^2\|u'''\|_{L^2(I)}.
$$

Define a quadratic interpolant on $I$ by integrating $q_I$ from the true left-endpoint value. The equal-average condition ensures that it reaches the true right-endpoint value, so these pieces join to an admissible continuous piecewise-quadratic function $I_hu$. Sum the squared estimates and use the best-approximation property:

$$
\boxed{\|u'-u_h'\|_2\leq\|u'-(I_hu)'\|_2\leq h^2\|u'''\|_2=h^2\|f'\|_2.}
$$

Only the maximum element length is used; equal spacing is unnecessary.

For the [Aubin–Nitsche duality argument](../../../../aubin-nitsche-duality-argument.md), let $e=u-u_h$ and solve $-z''=e$, $z(a)=0$, $z'(b)=0$. Explicitly $z'(x)=\int_x^be(t)\,dt$, so $\|z''\|_2=\|e\|_2$. Integration by parts and [Galerkin orthogonality](../../../../galerkin-orthogonality.md) give

$$
\|e\|_2^2=\int_a^be'z'\,dx=\int_a^be'[z'-(J_hz)']\,dx,
$$

where $J_hz$ is its nodal piecewise-linear interpolant, which belongs to the quadratic test space. On each element $(J_hz)'$ is the average of $z'$, so the same mean-zero inequality gives $\|z'-(J_hz)'\|_2\leq h\|z''\|_2$. Canceling $\|e\|_2$ when nonzero proves the additional order:

$$
\boxed{\|u-u_h\|_{L^2(a,b)}\leq h\|u'-u_h'\|_2\leq h^3\|f'\|_2.}
$$

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../split.md)
5. [Approximation theory and finite element methods course of the University of Oxford](../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
