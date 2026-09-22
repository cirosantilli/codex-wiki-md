<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use [left Grassmann derivatives](../../../../../left-grassmann-derivative.md) for the [Grassmann variables](../../../../../grassmann-variable.md). A [chiral superfield](../../../../../chiral-superfield.md) satisfies $\bar{\mathcal D}_{\dot\alpha}\Phi=0$. In the derivative convention printed in the PDF, differentiating $\theta\sigma^\mu\bar\theta$ with respect to a barred coordinate brings a minus sign from moving the odd derivative through $\theta$. Consequently $\bar{\mathcal D}_{\dot\alpha}y^\mu=0$, so the general solution depends only on $y$ and $\theta$:

$$
\boxed{\Phi(y,\theta)=\phi(y)+\sqrt2\,\theta\psi(y)+\theta^2F(y).}
$$

Here $\phi$ is a [complex scalar field](../../../../../complex-scalar-field.md), $\psi$ a [Weyl spinor](../../../../../weyl-spinor.md) and $F$ a complex [auxiliary field](../../../../../auxiliary-field.md). This is a finite [Grassmann algebra](../../../../../grassmann-algebra.md) expansion, not an assumption that the spacetime fields are constant.

For a completely convention-independent way to organize the ordinary-coordinate expansion, let $v^\mu=\theta\sigma^\mu\bar\theta$. Translation by $iv$ gives

$$
\Phi=\phi+\sqrt2\theta\psi+\theta^2F+iv^\mu\partial_\mu\phi+i\sqrt2\,v^\mu\theta\partial_\mu\psi-\frac12v^\mu v^\nu\partial_\mu\partial_\nu\phi.
$$

All higher terms vanish because there are only two unbarred and two barred odd coordinates. For example take $\sigma^\mu=(I,\boldsymbol\sigma)$, signature $(+---)$, $\theta^2=\theta^\alpha\theta_\alpha$ and $\bar\theta^2=\bar\theta_{\dot\alpha}\bar\theta^{\dot\alpha}$, with both lower epsilon tensors having $\epsilon_{12}=1$. Then $v^\mu v^\nu=\tfrac12\theta^2\bar\theta^2\eta^{\mu\nu}$ and the [chiral-superfield component expansion](../../../../../chiral-superfield-component-expansion.md) reads

$$
\boxed{\Phi=\phi+\sqrt2\theta\psi+\theta^2F+i\theta\sigma^\mu\bar\theta\,\partial_\mu\phi-\frac{i}{\sqrt2}\theta^2\partial_\mu\psi\sigma^\mu\bar\theta-\frac14\theta^2\bar\theta^2\Box\phi.}
$$

The frequently written positive quarter coefficient corresponds to the opposite convention for $\Box$ or the spinor contractions; the preceding shift formula fixes the sign without ambiguity. The local TeX's barred derivative is damaged: the original PDF has $\partial_\mu$, not a barred-coordinate factor at its end.

Write $X=x+\sqrt2\theta G+\theta^2F_X$ in chiral coordinates. Multiplication gives the three component constraints

$$
x^2=0,\qquad xG_\alpha=0,\qquad 2xF_X-GG=0.
$$

On the regular branch where the ordinary commuting part of $F_X$ is nonzero, the [nilpotent chiral superfield](../../../../../nilpotent-chiral-superfield.md) is therefore

$$
\boxed{X=\frac{GG}{2F_X}+\sqrt2\theta G+\theta^2F_X.}
$$

The [goldstino](../../../../../goldstino.md) $G$ and [auxiliary field](../../../../../auxiliary-field.md) $F_X$ are independent; the scalar is a composite, not another independent [degree of freedom](../../../../../degree-of-freedom.md). Its first two constraints follow because any product of three identical two-component odd spinor entries vanishes. It is essential not to divide by $F_X$ on a branch with zero commuting part: for example $X=0$ satisfies the nilpotency condition without breaking [supersymmetry](../../../../../supersymmetry-split.md).

For a regular local action with no superspace derivatives in $K$ or $W$, nilpotency truncates the most general [superpotential](../../../../../superpotential.md) and [Kähler potential](../../../../../kahler-potential.md) to

$$
\boxed{W=w_0+fX,\qquad K=k_0+k_1X+\overline{k_1}\bar X+\kappa X\bar X,\qquad k_0\in\mathbb R,\quad\kappa>0.}
$$

The last inequality makes the kinetic [Kähler metric](../../../../../kahler-metric.md) healthy. In global [four-dimensional N=1 supersymmetry](../../../../../four-dimensional-n-1-supersymmetry.md), the constant and holomorphic pieces of $K$ integrate to zero, and $w_0$ does not affect the action. On the bosonic background $G=0$, the constraint sets $x=0$ and the auxiliary terms are $\kappa F_X\bar F_X+fF_X+\bar f\bar F_X$. Eliminating them gives

$$
\boxed{F_X=-\frac{\bar f}{\kappa},\qquad V=\frac{|f|^2}{\kappa}.}
$$

A nonzero $f$ is necessary for this regular constrained branch to be an on-shell vacuum. It gives nonzero $F_X$ and [supersymmetry breaking](../../../../../supersymmetry-breaking.md), with $G$ the [goldstino](../../../../../goldstino.md). Nilpotency alone is not a proof that every possible branch breaks [supersymmetry](../../../../../supersymmetry-split.md). With $f=0$ the above composite parametrization is singular on shell, rather than evidence for a regular supersymmetric vacuum containing an independent [Goldstino](../../../../../goldstino.md).

If these data are instead embedded in [supergravity](../../../../../supergravity.md), the constant and linear terms cannot simply be discarded independently: a [Kähler transformation](../../../../../kahler-transformation.md) also transforms $W$. Before such a transformation, at $x=0$ the [supergravity F-term potential](../../../../../supergravity-f-term-potential.md) is

$$
V=e^{k_0}\left(\frac{|f+k_1w_0|^2}{\kappa}-3|w_0|^2\right),\qquad F^X=-e^{k_0/2}\frac{\overline{f+k_1w_0}}{\kappa}.
$$

Thus nonzero $F^X$ still breaks [supersymmetry](../../../../../supersymmetry-split.md), but the vacuum energy need not be positive. This distinguishes the global answer from the local theory explicitly introduced in the next question.

Now write $Y=y+\sqrt2\theta\chi+\theta^2F_Y$. The condition $XY=0$ becomes

$$
xy=0,\qquad x\chi_\alpha+yG_\alpha=0,\qquad xF_Y+yF_X-G\chi=0.
$$

Using the same nonzero-$F_X$ branch gives the [chiral superfield constrained by a nilpotent superfield](../../../../../chiral-superfield-constrained-by-a-nilpotent-superfield.md)

$$
\boxed{y=\frac{G\chi}{F_X}-\frac{GG}{2F_X^2}F_Y,\qquad Y=y+\sqrt2\theta\chi+\theta^2F_Y.}
$$

The spinor $\chi$ and the auxiliary $F_Y$ remain independent; the scalar is removed. Substituting this expression verifies the other two product constraints using two-component spinor identities. It does not impose $Y^2=0$. It does imply [cubic nilpotency from a mixed chiral constraint](../../../../../cubic-nilpotency-from-a-mixed-chiral-constraint.md): $Y^3=0$. Indeed $(G\chi)^2=-\tfrac12(GG)(\chi\chi)$, so

$$
y^2=-\frac{(GG)(\chi\chi)}{2F_X^2},\qquad y^3=0,\qquad y^2\chi=0,\qquad y^2F_Y-y\chi\chi=0.
$$

These are exactly the three components needed for $Y^3=0$. The generic nonzero expression for $y^2$ shows why imposing quadratic nilpotency on $Y$ would lose allowed interactions.

The analytic chiral monomials consequently reduce to $1,X,Y,Y^2$. The most general [superpotential](../../../../../superpotential.md) is

$$
\boxed{W=w_0+fX+gY+\frac m2Y^2.}
$$

For the [Kähler potential](../../../../../kahler-potential.md), put $U=(X,Y,Y^2)^T$. Every allowed mixed monomial is included in

$$
\boxed{K=k_0+\ell^TU+\overline{\ell^TU}+\sum_{a,b=1}^3h_{a\bar b}U_a\bar U_b,\qquad k_0\in\mathbb R,\quad h_{a\bar b}=\overline{h_{b\bar a}}.}
$$

This includes $X\bar X$, $X\bar Y$, $X\bar Y^2$, $Y\bar Y$, $Y\bar Y^2$, $Y^2\bar Y^2$ and the necessary conjugates; products containing $XY$ or $\bar X\bar Y$ vanish. In a global theory the holomorphic $\ell$ terms again integrate to zero; in [supergravity](../../../../../supergravity.md) they can be changed by a [Kähler transformation](../../../../../kahler-transformation.md). Positivity requires the kinetic metric on the independent multiplets to be positive definite at the chosen background, not necessarily the entire coefficient [matrix](../../../../../matrix.md) on the redundant composite list $U$. The most general claim here concerns regular analytic two-derivative actions; singular functions of the constrained fields or higher-derivative operators are outside it.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
