<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the standard Euclidean convention $e^{-S_E}$ and restore the curvature normalization explicitly. Let $\varphi$ be the conventional dimensionless [dilaton](../../../../../dilaton.md), whose worldsheet term is

$$
S_{\varphi}=\frac1{4\pi}\int_\Sigma d^2\sigma\sqrt h\,\varphi R^{(2)}.
$$

For constant $\varphi_0$, the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) gives $S_{\varphi}=\varphi_0\chi(\Sigma)$. A closed surface of genus $g$ has [Euler characteristic](../../../../../euler-characteristic.md) $\chi=2-2g$, so its contribution is weighted by

$$
e^{-S_{\varphi}}=e^{(2g-2)\varphi_0}=g_s^{2g-2}.
$$

Thus

$$
\boxed{g_s=e^{\varphi_0}.}
$$

This is the [dilaton normalization and Euler-characteristic weighting](../../../../../dilaton-normalization-and-euler-characteristic-weighting.md) of [string perturbation theory](../../../../../string-perturbation-theory.md). If the unit curvature coefficient in the printed expression is retained literally in this Euclidean convention, then $\varphi=4\pi\Phi$ and $g_s=e^{4\pi\Phi_0}$. If $\Phi$ denotes the conventional [dilaton](../../../../../dilaton.md), the usual omitted $1/(4\pi)$ is understood and $g_s=e^{\Phi_0}$. One must specify that normalization before exponentiating the field. Lorentzian overall signs are fixed consistently by Wick rotation.

For the [sigma-model beta function](../../../../../sigma-model-beta-function.md), use

$$
S_E=\frac1{4\pi\alpha'}\int d^2\sigma\,g_{ab}(X)\partial_\mu X^a\partial_\mu X^b
$$

with vanishing two-form and [dilaton](../../../../../dilaton.md). Perform the [background field expansion of a string sigma model](../../../../../background-field-expansion-of-a-string-sigma-model.md) covariantly by setting $X=\exp_{\bar X}\eta$. In [Riemann normal coordinates](../../../../../normal-coordinates.md), the quadratic fluctuation action is

$$
S^{(2)}=\frac1{4\pi\alpha'}\int d^2\sigma
\left[g_{ab}D_\mu\eta^aD_\mu\eta^b
-R_{acbd}\eta^a\eta^b\partial_\mu\bar X^c\partial_\mu\bar X^d\right].
$$

The covariant derivative contains the pulled-back target connection. This expansion accounts for the connection vertices as well as the normal-coordinate metric expansion; keeping only a single metric tadpole would not give a covariant answer.

Integrating the Gaussian fluctuations gives $\frac12\operatorname{Tr}\log\Delta$, where

$$
\Delta^a{}_b=-D^2\delta^a{}_b-R^a{}_{cbd}\partial_\mu\bar X^c\partial_\mu\bar X^d.
$$

Contracting the curvature vertex with the short-distance propagator traces $R^a{}_{cad}$ to the [Ricci tensor](../../../../../ricci-tensor.md) $R_{cd}$. In dimensional regularization at $d=2-\epsilon$, the logarithmic integral is $\int d^dp/(2\pi)^d(p^2+\mu^2)^{-1}=1/(2\pi\epsilon)+O(1)$. With the stated curvature convention the divergent effective action is

$$
\Gamma_{\rm div}^{(1)}=-\frac1{4\pi\epsilon}\int R_{ab}(\bar X)\partial_\mu\bar X^a\partial_\mu\bar X^b.
$$

It is cancelled by the metric counterterm $\delta g_{ab}=\alpha'R_{ab}/\epsilon$. Equivalently, write $g^{\rm bare}=\mu^{-\epsilon}(g+\alpha'R/\epsilon+\cdots)$. Differentiating the bare coupling at fixed value gives the [one-loop metric beta function of a string sigma model](../../../../../one-loop-metric-beta-function-of-a-string-sigma-model.md)

$$
\boxed{\beta^g_{ab}=\mu\frac{dg_{ab}}{d\mu}=\alpha'R_{ab}+O(\alpha'^2).}
$$

This loop is a loop of two-dimensional fluctuation fields: its expansion is in $\alpha\prime$, not a change of worldsheet genus or an extra power of $g_s$. The sign here defines the renormalization scale to increase toward the ultraviolet. For a round target sphere, positive Ricci curvature makes its squared radius increase with that scale, consistent with the usual asymptotic freedom of the inverse-radius sigma-model coupling. With the printed kinetic coefficient $1/2$ taken literally, $2\pi\alpha'=1$ and the leading coefficient is $R_{ab}/(2\pi)$. Requiring the metric beta function to vanish gives $R_{ab}=0$ at this order. Full bosonic-string Weyl consistency also requires the other anomaly coefficients, including the critical-dimension condition when the [dilaton](../../../../../dilaton.md) vanishes.

For [T-duality](../../../../../t-duality.md), choose coordinates $(y,x^i)$ adapted to the isometry and use $\alpha'=1$ units for the local [Buscher rules](../../../../../buscher-rules.md). Assume $g_{yy}\ne0$, with a spacelike isometry for the usual unitary circle duality. In light-cone worldsheet coordinates take the convention that $E=g+B$ multiplies $\partial_+X^a\partial_-X^b$. Gauge translations of $y$, replace $\partial_\pm y$ by $A_\pm$, gauge fix $y=0$, and impose flatness with a multiplier $\widetilde y$. The relevant first-order Lagrangian is

$$
\begin{aligned}
\mathcal L={}&g_{yy}A_+A_-+g_{yi}(A_+\partial_-x^i+\partial_+x^iA_-)
+g_{ij}\partial_+x^i\partial_-x^j\\
&+\widetilde y(\partial_+A_--\partial_-A_+).
\end{aligned}
$$

Integrating out $\widetilde y$ gives a locally pure-gauge connection and hence the original model. Instead integrate the last term by parts and solve the algebraic equations for $A_\pm$:

$$
A_+=\frac{\partial_+\widetilde y-g_{yi}\partial_+x^i}{g_{yy}},\qquad
A_-=-\frac{\partial_-\widetilde y+g_{yi}\partial_-x^i}{g_{yy}}.
$$

Substitution gives

$$
\begin{aligned}
\mathcal L'={}&\frac1{g_{yy}}\partial_+\widetilde y\partial_-\widetilde y
+\left(g_{ij}-\frac{g_{yi}g_{yj}}{g_{yy}}\right)\partial_+x^i\partial_-x^j\\
&+\frac{g_{yi}}{g_{yy}}\left(\partial_+\widetilde y\partial_-x^i-\partial_+x^i\partial_-\widetilde y\right).
\end{aligned}
$$

Reading its symmetric and antisymmetric parts yields the [Buscher dual of a metric with vanishing two-form](../../../../../buscher-dual-of-a-metric-with-vanishing-two-form.md):

$$
\boxed{g'_{yy}=\frac1{g_{yy}},\qquad g'_{yi}=0,\qquad
 g'_{ij}=g_{ij}-\frac{g_{yi}g_{yj}}{g_{yy}},}
$$



$$
\boxed{B'_{yi}=\frac{g_{yi}}{g_{yy}},\qquad B'_{iy}=-B'_{yi},\qquad B'_{ij}=0.}
$$

The spectator metric is the [Schur complement](../../../../../schur-complement.md) of $g_{yy}$. Reversing the orientation of $\widetilde y$ reverses the displayed mixed two-form signs; our multiplier and $E=g+B$ conventions fix them.

The metric rules arise already from the classical algebraic elimination. For quantum equivalence the regulated Gaussian measure also produces the [Buscher dilaton shift](../../../../../buscher-dilaton-shift.md)

$$
\varphi'=\varphi-\frac12\log g_{yy}.
$$

For a compact isometry the multiplier periodicity and flat-connection sectors implement the exchange of momentum and winding. On a circle, restoring dimensions gives **$R'=\alpha'/R$**. Thus the calculation derives the local dual background, while the measure and global sectors explain how it becomes a string-theory duality.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
