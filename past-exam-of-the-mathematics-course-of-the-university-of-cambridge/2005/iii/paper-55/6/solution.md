<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Work with metric $\eta=\operatorname{diag}(1,-1,-1,-1)$, $\sigma^\mu=(I,\boldsymbol\sigma)$ and $\bar\sigma^\mu=(I,-\boldsymbol\sigma)$, where $\boldsymbol\sigma$ are the [Pauli matrices](../../../../../pauli-matrices.md). The [supercharges](../../../../../supersymmetry-generator.md) of [four-dimensional N=1 supersymmetry](../../../../../four-dimensional-n-1-supersymmetry.md) form one [Weyl spinor](../../../../../weyl-spinor.md) $Q_\alpha$ and its conjugate $\bar Q_{\dot\alpha}$. Dotted and undotted indices cannot be interchanged; the conjugate charge in the printed mixed relation has a dotted index.

A direct derivation starts from [superspace](../../../../../superspace.md) coordinates $x^\mu,\theta^\alpha,\bar\theta^{\dot\alpha}$, with the four odd coordinates generating a [Grassmann algebra](../../../../../grassmann-algebra.md). Use left [Grassmann derivatives](../../../../../grassmann-derivative.md), so

$$
\partial_\alpha(\theta^\gamma f)=\delta_\alpha^\gamma f-\theta^\gamma\partial_\alpha f,
\qquad
\bar\partial_{\dot\beta}(\bar\theta^{\dot\gamma}f)
=\delta_{\dot\beta}^{\dot\gamma}f-\bar\theta^{\dot\gamma}\bar\partial_{\dot\beta}f.
$$

Odd derivatives anticommute with one another, and multiplication by distinct odd coordinates also anticommutes. The operators specified by the question can be written

$$
\mathcal P_\mu=-i\partial_\mu,\qquad
\mathcal Q_\alpha=-i\partial_\alpha
-\sigma^\mu_{\alpha\dot\gamma}\bar\theta^{\dot\gamma}\partial_\mu,
\qquad
\bar{\mathcal Q}_{\dot\beta}=i\bar\partial_{\dot\beta}
+\theta^\gamma\sigma^\mu_{\gamma\dot\beta}\partial_\mu.
$$

Their coefficients do not depend on $x$, hence $[\mathcal Q_\alpha,\mathcal P_\mu]=[\bar{\mathcal Q}_{\dot\alpha},\mathcal P_\mu]=0$. Within $\{\mathcal Q_\alpha,\mathcal Q_\beta\}$, the two odd derivative terms anticommute; the derivatives of the barred-coordinate coefficients vanish; and the two barred-coordinate multiplication terms cancel because the coordinates anticommute while the spacetime derivatives commute. Thus

$$
\{\mathcal Q_\alpha,\mathcal Q_\beta\}=0,
\qquad
\{\bar{\mathcal Q}_{\dot\alpha},\bar{\mathcal Q}_{\dot\beta}\}=0.
$$

This realizes the minimal algebra with no extra tensorial charges.

For the mixed [anticommutator](../../../../../anticommutator.md), split each operator into its odd derivative and odd-coordinate parts. The derivative/derivative anticommutator is zero. The coordinate/coordinate terms also cancel, since $\theta\bar\theta=-\bar\theta\theta$. The two remaining pieces are

$$
\{-i\partial_\alpha,\ \theta^\gamma\sigma^\mu_{\gamma\dot\beta}\partial_\mu\}
=-i\sigma^\mu_{\alpha\dot\beta}\partial_\mu,
$$



$$
\{-\sigma^\mu_{\alpha\dot\gamma}\bar\theta^{\dot\gamma}\partial_\mu,
\ i\bar\partial_{\dot\beta}\}
=-i\sigma^\mu_{\alpha\dot\beta}\partial_\mu.
$$

Adding gives the [superspace differential realization of N=1 supercharges](../../../../../superspace-differential-realization-of-n-1-supercharges.md):

$$
\boxed{\{\mathcal Q_\alpha,\bar{\mathcal Q}_{\dot\beta}\}
=-2i\sigma^\mu_{\alpha\dot\beta}\partial_\mu
=2\sigma^\mu_{\alpha\dot\beta}\mathcal P_\mu.}
$$

In particular the differentiated-coordinate contributions have the same sign, not opposite signs. The graded product rule is the essential step; treating these as ordinary commuting-coordinate derivatives would give an incorrect algebra.

To obtain the Lorentz part, let $x$ transform as a four-vector and $\theta,\bar\theta$ in conjugate spinor representations. Define

$$
\Sigma^{\mu\nu}=\frac14(\sigma^\mu\bar\sigma^\nu-\sigma^\nu\bar\sigma^\mu),
\qquad
\bar\Sigma^{\mu\nu}=\frac14(\bar\sigma^\mu\sigma^\nu-\bar\sigma^\nu\sigma^\mu).
$$

The [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) gives the intertwining identity

$$
\Sigma^{\mu\nu}\sigma^\rho-\sigma^\rho\bar\Sigma^{\mu\nu}
=\eta^{\nu\rho}\sigma^\mu-\eta^{\mu\rho}\sigma^\nu.
$$

It shows that the two terms in $\mathcal Q_\alpha$ transform together as a covariant [Weyl spinor](../../../../../weyl-spinor.md): the coordinate derivative transforms in the dual spinor representation, while the barred-coordinate/spacetime-derivative term transforms in that same representation through this identity. Infinitesimally, with $U=\exp[-\tfrac i2\omega_{\mu\nu}M^{\mu\nu}]$, its transformation is $UQ_\alpha U^{-1}=Q_\alpha-\tfrac12\omega_{\mu\nu}(\Sigma^{\mu\nu})_\alpha{}^\beta Q_\beta$. Comparing with the first-order expansion of $U$ gives

$$
[Q_\alpha,M^{\mu\nu}]=i(\Sigma^{\mu\nu})_\alpha{}^\beta Q_\beta.
$$

If the paper's spin matrix is denoted $\sigma^{\mu\nu}=i\Sigma^{\mu\nu}$, this is exactly its first displayed relation. Defining that spin matrix without the factor $i$ instead requires an explicit $i$ in the commutator; this is a generator convention, not a different algebra. The conjugate relation follows by Hermitian conjugation.

Combining the Lorentz transformation with the differential computations gives the [Super-Poincaré algebra](../../../../../super-poincare-algebra.md) in the question's notation:

$$
\boxed{[Q_\alpha,M^{\mu\nu}]=(\sigma^{\mu\nu})_\alpha{}^\beta Q_\beta,\quad
[Q_\alpha,P^\mu]=0,\quad\{Q_\alpha,Q_\beta\}=0,\quad
\{Q_\alpha,\bar Q_{\dot\beta}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu.}
$$

The even generators retain the ordinary [Poincare algebra](../../../../../poincare-algebra.md). As a closure check, the even superspace variation $\delta=i(\epsilon\mathcal Q-\bar\epsilon\bar{\mathcal Q})$ gives $\delta\theta=\epsilon$, $\delta\bar\theta=\bar\epsilon$ and $\delta x^\mu=i\theta\sigma^\mu\bar\epsilon-i\epsilon\sigma^\mu\bar\theta$. Two such variations commute to a translation by $2i(\epsilon_1\sigma^\mu\bar\epsilon_2-\epsilon_2\sigma^\mu\bar\epsilon_1)$, with zero commutator on the odd coordinates, reproducing the same normalization and showing why the anticommutator produces momentum.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
