<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

A fixed-step [linear multistep method](../../../../../linear-multistep-method.md) for $y'=f(t,y)$ uses several previous solution and derivative values:

$$
\sum_{j=0}^s\alpha_jy_{n+j}
=k\sum_{j=0}^s\beta_jf(t_{n+j},y_{n+j}),\qquad \alpha_s\ne0.
$$

The coefficients are fixed independently of the step size. It is explicit when $\beta_s=0$ and implicit otherwise. Its [characteristic polynomials of a linear multistep method](../../../../../characteristic-polynomials-of-a-linear-multistep-method.md) are $\rho(w)=\sum_j\alpha_jw^j$ and $\sigma(w)=\sum_j\beta_jw^j$. The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) gives a uniquely solvable implicit step under a [Lipschitz continuity](../../../../../lipschitz-continuity.md) bound $L$ whenever $k|\beta_s|L<|\alpha_s|$, by contraction of the new-value equation on the appropriate solution region. A suitable starting procedure must supply the first $s$ values; the method alone does not determine them.

Order is defined by inserting a smooth exact solution into the recurrence. If the residual is $O(k^{p+1})$ and its first nonzero coefficient occurs at that degree, the method has order $p$; dividing the residual by $k$ gives an $O(k^p)$ [local truncation error](../../../../../local-truncation-error.md). [Taylor expansion](../../../../../taylor-expansion.md) gives the exact [order conditions for a linear multistep method](../../../../../order-conditions-for-a-linear-multistep-method.md)

$$
\sum_j\alpha_jj^q=q\sum_j\beta_jj^{q-1}\quad(0\leq q\leq p),
$$

with the right side interpreted as zero at $q=0$, and failure at $q=p+1$ for exact order. Equivalently,

$$
\rho(e^z)-z\sigma(e^z)=O(z^{p+1}).
$$

The basic [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) conditions are $\rho(1)=0$, $\rho'(1)=\sigma(1)$; for the ordinary nondegenerate consistent formulation this common value is nonzero. Exactness on constants and linear functions does not control propagation of numerical perturbations.

That propagation is the role of [zero-stability](../../../../../zero-stability.md). On $y'=0$ the homogeneous recurrence is $\rho(E)y_n=0$. Its modes are $n^r\xi^n$, with powers of $n$ determined by root multiplicities. The theorem on the [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md) states that [zero-stability](../../../../../zero-stability.md) is equivalent to every root of $\rho$ having modulus at most one, with every unit-modulus root simple. Interior repeated roots are permitted, since geometric decay dominates their [polynomial](../../../../../polynomial-split.md) factors. An exterior root amplifies perturbations geometrically; a repeated unit root amplifies them polynomially and violates a step-independent perturbation bound.

The [Dahlquist equivalence theorem](../../../../../dahlquist-equivalence-theorem.md) states that a fixed-step consistent [linear multistep method](../../../../../linear-multistep-method.md) is convergent exactly when it is [zero-stable](../../../../../zero-stability.md). This concerns [ordinary differential equations](../../../../../ordinary-differential-equation.md) with a uniformly [Lipschitz continuous](../../../../../lipschitz-continuity.md) right-hand side on the solution region over a fixed finite interval, convergent starting values, and the well-defined nearby branch of each small-step implicit solve. For order $p$ [convergence of a numerical method](../../../../../convergence-of-a-numerical-method.md), the solution must have the required smoothness and the starting errors must be $O(k^p)$.

The mechanism can be sketched explicitly. The [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md) bounds the recurrence's discrete [Green function](../../../../../green-s-function.md). For an order-$p$ exact-solution defect $d_n=O(k^{p+1})$, the [Lipschitz continuity](../../../../../lipschitz-continuity.md) error equation then gives an estimate of the form

$$
E_n\leq C\left(E_{\mathrm{start}}+\sum_{j<n}\|d_j\|\right)
+Ck\sum_{j\leq n}E_j.
$$

The current-step term can be absorbed for small $k$. The [discrete Gronwall inequality](../../../../../discrete-gronwall-inequality.md) says that a bound $E_n\leq A+Bk\sum_{j<n}E_j$ implies $E_n\leq A(1+Bk)^n\leq Ae^{Bt_n}$. There are $O(k^{-1})$ defects on a fixed interval, so their sum is $O(k^p)$ and this yields the claimed global order. Conversely, testing $y'=0$ with vanishing starting perturbations in exterior-root or repeated-unit-root modes proves that [convergence of a numerical method](../../../../../convergence-of-a-numerical-method.md) fails without the [root condition for a multistep method](../../../../../root-condition-for-a-multistep-method.md).

For example, the two-step [Adams-Bashforth method](../../../../../adams-bashforth-method.md) has

$$
y_{n+2}-y_{n+1}=k(3f_{n+1}-f_n)/2,
\qquad \rho=w(w-1),\quad\sigma=(3w-1)/2.
$$

It is explicit, order two and [zero-stable](../../../../../zero-stability.md), hence convergent with order-two starting values. By contrast, a recurrence with $\rho=(w-1)^2$ has solutions $y_n=y_0+n(y_1-y_0)$ on the zero differential equation. Starting differences $\sqrt k$ tend to zero yet become unbounded at a fixed positive time, since $n$ is of order $1/k$. A small local defect or formal high order cannot rescue this mode. Canceling a common factor may remove it only by changing the allowed starting relations, as the parameter endpoint in Question 2 illustrates.

[Absolute stability](../../../../../linear-stability-domain.md) addresses a different limit: apply the method to the [Dahlquist test equation](../../../../../dahlquist-test-equation.md) $y'=\lambda y$ and put $z=k\lambda$. The amplification roots satisfy

$$
P_z(w)=\rho(w)-z\sigma(w)=0.
$$

All roots must satisfy the disk condition, with unit roots simple; one cannot inspect only the root that tends to one as $z\to0$. The degree and solvability of the recurrence must also be preserved. The resulting set of $z$ is the domain of [absolute stability](../../../../../linear-stability-domain.md). [A-stability](../../../../../a-stability.md) means that it includes the whole closed left half-plane, so the numerical solutions of every [Dahlquist test equation](../../../../../dahlquist-test-equation.md) with $\operatorname{Re}\lambda\leq0$ are stable for every positive step size. It is a linear test-equation property, not a proof of arbitrary nonlinear contractivity or high accuracy at large steps.

[Forward Euler method](../../../../../euler-method.md) has order one and factor $1+z$, so its stability region is the disk $|1+z|\leq1$. [Backward Euler method](../../../../../backward-euler-method.md) has factor $(1-z)^{-1}$ and is [A-stable](../../../../../a-stability.md). The [trapezoidal rule](../../../../../trapezoidal-rule.md) is order two with factor $(1+z/2)/(1-z/2)$; its modulus is at most one throughout the left half-plane. These one-step methods are included as the simplest multistep examples. For the two-step [Adams-Bashforth method](../../../../../adams-bashforth-method.md), the negative-real stability interval is $-1\leq z\leq0$: its [polynomial](../../../../../polynomial-split.md) is $w^2-(1+3z/2)w+z/2$, and the root reaches $-1$ at $z=-1$. It therefore imposes a step restriction when applied to strongly decaying modes.

The genuinely two-step [BDF2 method](../../../../../second-order-backward-differentiation-formula.md) is

$$
3y_{n+2}-4y_{n+1}+y_n=2k f_{n+2}.
$$

It has order two, roots $1,1/3$ at zero step and is [A-stable](../../../../../a-stability.md). For its normalized [polynomials](../../../../../polynomial-split.md) $\rho=3w^2/2-2w+1/2$, $\sigma=w^2$, the unit-circle boundary locus has

$$
\operatorname{Re}\frac{\rho(e^{i\theta})}{\sigma(e^{i\theta})}
=(1-\cos\theta)^2\geq0.
$$

The leading coefficient has no zero in the left half-plane, and the roots at a small negative $z$ are both inside the disk. Root continuity then proves open-half-plane stability; on the imaginary boundary the only possible unit root is the simple root one at $z=0$. This gives a direct proof of the stated [A-stability](../../../../../a-stability.md) rather than relying on a boundary plot.

Two sharp order barriers explain the tradeoff. The [first Dahlquist barrier](../../../../../first-dahlquist-barrier.md) states that a consistent [zero-stable](../../../../../zero-stability.md) real linear $s$-step method using only first derivatives has order at most $s+1$ for odd $s$ and $s+2$ for even $s$; an explicit method has order at most $s$. The [Second Dahlquist barrier](../../../../../second-dahlquist-barrier.md) states that an irreducible [A-stable](../../../../../a-stability.md) real [linear multistep method](../../../../../linear-multistep-method.md) has order at most two. These statements concern fixed constant coefficients and the ordinary first-derivative multistep class, not multiderivative methods or arbitrary variable-step formulations. Thus higher order alone is not a route to unconditional stiff stability. Question 2 provides a concrete illustration: its third-order member is [zero-stable](../../../../../zero-stability.md) but not [A-stable](../../../../../a-stability.md).

No nontrivial consistent explicit [multistep method](../../../../../linear-multistep-method.md) is [A-stable](../../../../../a-stability.md). Its [amplification polynomial of a multistep method](../../../../../amplification-polynomial-of-a-multistep-method.md) has a fixed highest coefficient, while at least one lower coefficient grows without bound as real $z\to-\infty$. Were all roots uniformly in the [unit disk](../../../../../unit-disk.md), their [elementary symmetric polynomials](../../../../../elementary-symmetric-polynomial.md) would keep all the monic coefficients bounded, a contradiction. This is the coefficient argument behind [explicit multistep methods cannot be A-stable](../../../../../explicit-multistep-methods-cannot-be-a-stable.md).

In practice, selecting a method therefore involves accuracy, startup, the presence of a [stiff differential equation](../../../../../stiff-equation.md), implicit-solve cost and step-size control. [Zero-stability](../../../../../zero-stability.md) handles propagation as the step tends to zero; [consistency of a numerical method](../../../../../consistency-of-a-numerical-method.md) supplies a vanishing defect; [A-stability](../../../../../a-stability.md) handles the numerical solutions of all decaying [Dahlquist test equations](../../../../../dahlquist-test-equation.md) at finite steps. None substitutes for the others, and variable steps or PDE discretizations require additional uniform stability arguments appropriate to their setting.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
