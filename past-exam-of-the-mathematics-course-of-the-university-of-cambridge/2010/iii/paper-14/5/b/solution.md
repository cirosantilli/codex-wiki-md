<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

We use the following precise degree-zero/one [kernel of the magnetic X-ray transform in degrees zero and one](../../../../../../kernel-of-the-magnetic-x-ray-transform-in-degrees-zero-and-one.md) theorem, as permitted here: for a smooth Anosov [magnetic flow](../../../../../../magnetic-flow-on-a-riemannian-surface.md) on a closed oriented surface, if

$$
Fh=q(x)+\xi_x(v),\qquad h\in C^\infty(SM),
$$

with $q$ a smooth base function and $\xi$ a smooth [one-form](../../../../../../one-form.md), then $q=0$ and $\xi$ is exact. Exact [one-forms](../../../../../../one-form.md) give the converse, because $F(w\circ\pi)=dw(v)$. No assumption of pointwise negative Gaussian curvature is needed for this theorem. We now derive the contact obstruction from it rather than assume the desired rigidity conclusion.

Use the usual connected-surface convention. Since $\int_M f\Omega_a=0$, the top-degree [de Rham cohomology](../../../../../../de-rham-cohomology.md) class of $f\Omega_a$ vanishes: integration identifies $H^2_{\mathrm{dR}}(M)$ with $\mathbb R$. Choose a smooth [one-form](../../../../../../one-form.md) $\eta$ on $M$ satisfying $d\eta=f\Omega_a$, and set

$$
\sigma=\alpha-\pi^*\eta.
$$

The structure equations and the previous volume calculation give

$$
d\sigma=d\alpha-f\pi^*\Omega_a=-\iota_F\mu,
\qquad \sigma(F)=1-\eta_x(v).
$$

This primitive exists because of the zero-flux hypothesis, and need not itself be contact.

A useful elementary fact is that every [smooth invariant function of an Anosov flow](../../../../../../smooth-invariant-function-of-an-anosov-flow.md) is constant on a connected manifold. If $Fh=0$, then $dh_x(v_s)=dh_{\phi_t x}(D\phi_t v_s)$, and boundedness of $dh$ with exponential contraction makes this zero as $t\to\infty$. Negative time does the same for an unstable vector. Also $dh(F)=0$. The Anosov splitting spans the tangent space, so $dh=0$. This avoids any extra ergodicity assumption.

Suppose a smooth [contact form](../../../../../../contact-form.md) $\tau$ is preserved. Invariance and contraction imply $\tau(v_s)=\tau(D\phi_t v_s)=0$ in the limit; negative time gives the same on unstable vectors. Thus $\tau$ annihilates both transverse bundles. Its value $\tau(F)$ cannot vanish anywhere, since otherwise $\tau$ would be zero at that point, contradicting the contact condition. It is a smooth invariant function and therefore a nonzero constant. Divide $\tau$ by that constant to arrange $\tau(F)=1$.

The [Cartan formula for the Lie derivative](../../../../../../cartan-s-magic-formula.md) now gives $\iota_Fd\tau=0$. In dimension three, all two-forms annihilating $F$ are scalar multiples of $\iota_F\mu$, so

$$
d\tau=k\,\iota_F\mu.
$$

The scalar $k$ is smooth and nowhere zero by the contact condition. Both sides without $k$ are flow-invariant; hence $Fk=0$ and the preceding Anosov argument makes $k$ constant. It follows that

$$
\zeta:=\tau+k\sigma
$$

is a [closed differential one-form](../../../../../../closed-differential-one-form.md).

We require the Liouville mean of such a [closed differential form](../../../../../../closed-differential-form.md), and derive it explicitly. Let $R_s$ be fibre rotation and average $\zeta$ over $0\le s\le2\pi$. Since $d\zeta=0$, the [Cartan formula for the Lie derivative](../../../../../../cartan-s-magic-formula.md) gives

$$
R_s^*\zeta-\zeta=d\left(\int_0^sR_r^*(\zeta(V))\,dr\right).
$$

Consequently its rotational average differs from $\zeta$ by an exact form. For a closed rotationally invariant [one-form](../../../../../../one-form.md) $\overline\zeta$, the identity $d(\overline\zeta(V))=\mathcal L_V\overline\zeta-\iota_Vd\overline\zeta=0$ makes its vertical value a constant $a$. Subtracting $a\omega$ leaves a rotationally invariant horizontal form, which descends to a base form $\xi$. We have therefore proved the [averaging closed one-forms on a surface unit tangent bundle](../../../../../../averaging-closed-one-forms-on-a-surface-unit-tangent-bundle.md) decomposition

$$
\zeta=\pi^*\xi+a\omega+dh,
\qquad d\xi=aK\Omega_a.
$$

The last relation follows from closedness and $d\omega=-K\pi^*\Omega_a$.

Evaluation at $F$ gives $\zeta(F)=\xi_x(v)+af+Fh$. The average of the linear expression $\xi_x(v)$ around each unit circle is zero. The second term has total integral $2\pi a\int_M f\Omega_a=0$. Finally $\int_{SM}Fh\,d\mu=0$ by volume preservation and [Stokes theorem](../../../../../../stokes-theorem.md). Thus

$$
\int_{SM}\zeta(F)\,d\mu=0
$$

for every [closed differential one-form](../../../../../../closed-differential-one-form.md) $\zeta$ in this zero-flux system. Apply this to $\tau+k\sigma$: the directional average of $\eta_x(v)$ also vanishes, so its integral is $(1+k)\operatorname{Vol}_\mu(SM)$. Positivity of the volume forces $k=-1$. Hence $d\tau=d\sigma$ and $\zeta=\tau-\sigma$ is closed.

Using its proved decomposition and $\tau(F)=1$, we obtain

$$
1=1-\eta_x(v)+\xi_x(v)+af+Fh,
\qquad \boxed{Fh=(\eta-\xi)_x(v)-af}.
$$

The stated magnetic transform kernel theorem gives $af=0$ and exactness of $\eta-\xi$, hence $d\eta=d\xi$. If $a=0$, then $d\xi=0$ and $f\Omega_a=d\eta=0$, so $f=0$. If $a\ne0$, the equation $af=0$ already gives $f=0$. Necessity is proved.

Conversely, if $f=0$, then $F=X$. The canonical form $\alpha$ is contact because $\alpha\wedge d\alpha=-\mu$ never vanishes, and

$$
\mathcal L_X\alpha=\iota_Xd\alpha+d(\alpha(X))=0+d1=0.
$$

Thus the flow preserves $\alpha$, proving

$$
\boxed{\phi_t\text{ preserves a smooth contact form}\quad\Longleftrightarrow\quad f\equiv0}.
$$

If disconnected surfaces are admitted, the flux condition must hold on each component for the exactness step; a single cancelling total flux does not imply componentwise exactness. The result above uses the standard connected interpretation of a surface.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
