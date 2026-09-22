<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

On a [complex manifold](../../../../../complex-manifold.md), the [exterior derivative](../../../../../exterior-derivative.md) splits by type as $d=\partial+\bar\partial$. The [conjugate Dolbeault operator](../../../../../conjugate-dolbeault-operator.md) $\partial$ raises [holomorphic](../../../../../complex-differentiability-at-a-point.md) degree by one and the [Dolbeault operator](../../../../../dolbeault-operator.md) $\bar\partial$ raises antiholomorphic degree by one. Their identities are

$$
\partial^2=\bar\partial^2=0,\qquad\partial\bar\partial+\bar\partial\partial=0.
$$

Use the convention $d^c=i(\bar\partial-\partial)$ for the [d c operator](../../../../../d-c-operator.md); then $dd^c=2i\partial\bar\partial$. The alternative convention with a factor $1/2$ changes this last factor only. [Complex conjugation of differential-form type](../../../../../complex-conjugation-of-differential-form-type.md) interchanges $\partial$ and $\bar\partial$ without reversing the wedge order. Thus, for a real form $\eta$,

$$
\overline{i\partial\bar\partial\eta}=-i\bar\partial\partial\eta=i\partial\bar\partial\eta.
$$

**The resulting form is real**, independently of the degree or type components of $\eta$.

The [Dolbeault cohomology](../../../../../dolbeault-cohomology.md) is

$$
H^{p,q}(X)=\frac{\ker(\bar\partial:\mathcal A^{p,q}\to\mathcal A^{p,q+1})}{\operatorname{im}(\bar\partial:\mathcal A^{p,q-1}\to\mathcal A^{p,q})}.
$$

In degree $(0,0)$ there is no incoming image, and the kernel consists of global [holomorphic functions](../../../../../holomorphic-function.md). On a [compact](../../../../../compact-space.md) [connected](../../../../../connected-space.md) $X$, $|f|$ attains a maximum. In a coordinate polydisc around a maximizing point, the one-variable [maximum modulus principle](../../../../../maximum-modulus-principle.md) applied successively along the coordinate directions makes $f$ constant on a smaller polydisc. Alternatively the same argument shows the maximum set is open; it is closed and nonempty, so [connectedness](../../../../../connected-space.md) makes it all of $X$, and the local constancy then makes $f$ globally constant. Consequently

$$
\boxed{H^{0,0}(X)\cong\mathbb C.}
$$

A [holomorphic p-form on a complex manifold](../../../../../holomorphic-p-form-on-a-complex-manifold.md) is a form of type $(p,0)$ with [holomorphic coordinate](../../../../../holomorphic-coordinate.md) coefficients, equivalently one killed by $\bar\partial$. For degree $n=\dim_{\mathbb C}X$, it is $d$-closed: its $\bar\partial$ vanishes by holomorphicity and its $\partial$ has impossible bidegree $(n+1,0)$. Its conjugate is also closed.

The key positivity behind [nonzero holomorphic top forms are not exact](../../../../../nonzero-holomorphic-top-forms-are-not-exact.md) is explicit. If $\alpha=f\,dz_1\wedge\cdots\wedge dz_n$, complex orientation gives

$$
i^{n^2}\alpha\wedge\bar\alpha
=2^n|f|^2\,dx_1\wedge dy_1\wedge\cdots\wedge dx_n\wedge dy_n.
$$

This is nonnegative everywhere and positive on some open set when $\alpha\not\equiv0$, so its integral on the [compact](../../../../../compact-space.md) manifold is strictly positive. If $\alpha=d\gamma$, closedness of $\bar\alpha$ and the [Stokes theorem](../../../../../stokes-theorem.md) would give

$$
\int_X\alpha\wedge\bar\alpha=\int_Xd(\gamma\wedge\bar\alpha)=0.
$$

Here Stokes is used on a [compact](../../../../../compact-space.md) oriented manifold without boundary, and complex-valued forms are handled by linearity. The contradiction proves **a nonzero [holomorphic](../../../../../complex-differentiability-at-a-point.md) top form is not $d$-exact**. For dimension zero the same nonexactness follows directly from the absence of degree $-1$ forms.

Now take a [compact](../../../../../compact-space.md) [complex surface](../../../../../complex-surface.md), with no [Kähler metric](../../../../../kahler-metric.md) assumed. For a [holomorphic](../../../../../complex-differentiability-at-a-point.md) one-form $\alpha$, the form $\beta=d\alpha=\partial\alpha$ has type $(2,0)$ and is [holomorphic](../../../../../complex-differentiability-at-a-point.md), since $\bar\partial\partial\alpha=-\partial\bar\partial\alpha=0$. It is exact. The top-form result forces $\beta=0$, proving closedness. This establishes [holomorphic forms on a compact complex surface are closed](../../../../../holomorphic-forms-on-a-compact-complex-surface-are-closed.md) by an argument which does not require a Kähler identity.

If a [holomorphic](../../../../../complex-differentiability-at-a-point.md) one-form were exact, write $\alpha=df$ for a global smooth complex function. Comparing types gives $\bar\partial f=0$. The preceding [compactness](../../../../../compact-space.md) argument makes $f$ constant on every [connected](../../../../../connected-space.md) component, hence $\alpha=0$. [Holomorphic](../../../../../complex-differentiability-at-a-point.md) two-forms are closed and nonexact unless zero by the top-form result. [Holomorphic](../../../../../complex-differentiability-at-a-point.md) zero-forms are constant on each component, and a nonzero zero-form is never exact because there are no negative-degree forms. Degrees above two contain only zero forms. Therefore **every [holomorphic](../../../../../complex-differentiability-at-a-point.md) form on a [compact](../../../../../compact-space.md) complex surface is closed, and a nonzero one is never exact**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
