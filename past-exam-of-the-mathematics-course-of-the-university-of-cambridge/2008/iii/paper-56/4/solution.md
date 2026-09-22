<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the scalar components of the three [chiral superfields](../../../../../chiral-superfield.md), and set $a=|\phi_0|^2$, $b=|\phi_+|^2$, $c=|\phi_-|^2$ and $\Sigma=a+b+c$. We assume the physical sign $g>0$ and a nonzero coupling $\lambda$. The coefficient $g$ below is exactly the coefficient in the supplied [D-term scalar potential](../../../../../d-term-scalar-potential.md); it should not be silently replaced by a differently normalized squared [gauge coupling](../../../../../gauge-coupling.md). The canonical [Kähler potential](../../../../../kahler-potential.md) has identity [Kähler metric](../../../../../kahler-metric.md), and the three [Kähler covariant derivatives of a superpotential](../../../../../kahler-covariant-derivative-of-a-superpotential.md) are

$$
\begin{aligned}
D_0W&=\lambda\phi_+\phi_-(1+\kappa^2a),\\
D_+W&=\lambda\phi_0\phi_-(1+\kappa^2b),\\
D_-W&=\lambda\phi_0\phi_+(1+\kappa^2c).
\end{aligned}
$$

Substitution in the [supergravity F-term potential](../../../../../supergravity-f-term-potential.md) gives

$$
\begin{aligned}
V_F={}&|\lambda|^2e^{\kappa^2\Sigma}
\left[bc(1+\kappa^2a)^2+ac(1+\kappa^2b)^2
+ab(1+\kappa^2c)^2-3\kappa^2abc\right]\\
={}&|\lambda|^2e^{\kappa^2\Sigma}
\left[ab+ac+bc+3\kappa^2abc+\kappa^4abc\Sigma\right].
\end{aligned}
$$

In particular, the subtraction cancels only half of the six $\kappa^2abc$ terms contributed by the three squares. The full [scalar potential](../../../../../scalar-potential.md) is

$$
\boxed{V=|\lambda|^2e^{\kappa^2\Sigma}
\left[ab+ac+bc+3\kappa^2abc+\kappa^4abc\Sigma\right]
+g(b-c-\zeta)^2\ge0.}
$$

Its nonnegativity follows term by term from $a,b,c\ge0$ and $g>0$. This is a special property of this cubic [superpotential](../../../../../superpotential.md), not of a general [supergravity F-term potential](../../../../../supergravity-f-term-potential.md).

The [D-term vacuum branches of a cubic superpotential](../../../../../d-term-vacuum-branches-of-a-cubic-superpotential.md) must be described as branches: there are not two isolated field-space minima. First suppose $\zeta>0$. Vanishing of $V_F$ requires $ab=ac=bc=0$, and vanishing of the [D-term scalar potential](../../../../../d-term-scalar-potential.md) requires $b-c=\zeta$. Together these conditions give the [vacuum expectation values](../../../../../vacuum-expectation-value.md)

$$
\boxed{\langle\phi_0\rangle=\langle\phi_-\rangle=0,
\qquad |\langle\phi_+\rangle|=\sqrt\zeta,
\qquad V=0.}
$$

The phase of $\phi_+$ lies on a [gauge orbit](../../../../../gauge-orbit.md), and one may choose it positive and real. At this [global minimum](../../../../../global-minimum.md), all $D_iW$ and the real [auxiliary field](../../../../../auxiliary-field.md) of the [vector multiplet](../../../../../supersymmetric-vector-multiplet.md) vanish. It is a [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md), even though the internal [gauge symmetry](../../../../../gauge-invariance.md) is spontaneously broken. For $\zeta<0$, interchange $\phi_+$ and $\phi_-$: the nonzero [vacuum expectation value](../../../../../vacuum-expectation-value.md) has magnitude $\sqrt{-\zeta}$. For $\zeta=0$, the [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) is the entire family $\phi_+=\phi_-=0$, with $\phi_0$ arbitrary.

The other branch has $\phi_+=\phi_-=0$ and arbitrary $\phi_0$. Here $W=D_iW=0$ but the real [auxiliary field](../../../../../auxiliary-field.md) is nonzero for $\zeta\ne0$, and

$$
V=g\zeta^2.
$$

Thus this branch has pure [D-term](../../../../../d-term.md) [supersymmetry breaking](../../../../../supersymmetry-breaking.md) and a [flat direction of a scalar potential](../../../../../flat-direction-of-a-scalar-potential.md) in the neutral scalar. It is not stable at every neutral-field value. At a fixed $a=|\phi_0|^2$, expansion in the charged scalars yields

$$
V=g\zeta^2
+\left(|\lambda|^2ae^{\kappa^2a}-2g\zeta\right)|\phi_+|^2
+\left(|\lambda|^2ae^{\kappa^2a}+2g\zeta\right)|\phi_-|^2
+O\left((b+c)^2\right).
$$

Hence the two charged squared [masses](../../../../../mass.md) and the stability condition are

$$
\boxed{m_\pm^2=|\lambda|^2ae^{\kappa^2a}\mp2g\zeta,
\qquad |\lambda|^2ae^{\kappa^2a}>2g|\zeta|.}
$$

Above this threshold, both charged directions have positive [mass](../../../../../mass.md) squared. Continuity makes them uniformly positive in a sufficiently small neighborhood of the chosen neutral-field value, so the stationary branch is a genuine, non-strict [local minimum](../../../../../local-minimum.md) valley. Its neutral direction stays flat. Below the threshold, a charged [mass](../../../../../mass.md) squared is negative and the branch is a [saddle point](../../../../../saddle-point.md). At equality it is a boundary of the stable valley, not a [local minimum](../../../../../local-minimum.md) in the full field space: changing $a$ slightly downward and switching on the unstable charged field lowers $V$. For example, for $\zeta>0$, put $a=a_c-\epsilon$, $b=\epsilon^2$, $c=0$. Since $M(a)=|\lambda|^2ae^{\kappa^2a}$ has $M'(a_c)>0$, one finds $V-g\zeta^2=-M'(a_c)\epsilon^3+O(\epsilon^4)<0$.

There are no further local-minimum branches under these generic assumptions. If $b+c>0$, the expression for $V_F$ is strictly increasing in $a$, so a stationary configuration with a charged condensate must have $a=0$. At $a=0$, an interior critical point with $b,c>0$ is impossible, because

$$
\partial_b V+\partial_c V
=|\lambda|^2e^{\kappa^2(b+c)}
\left(b+c+2\kappa^2bc\right)>0.
$$

On the boundary $c=0$, the relevant [scalar potential](../../../../../scalar-potential.md) is $g(b-\zeta)^2$; on $b=0$ it is $g(c+\zeta)^2$. Their nonnegative-domain minima give exactly the [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) described above, or the origin of the charged-field branch. Thus, for nonzero $\zeta$, **the two types are the zero-energy supersymmetric gauge orbit and the positive-energy D-breaking minimum valley above the threshold**. If $\zeta=0$, the two types coalesce into the flat [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md); the literal two-minimum assertion needs this parameter qualification.

In the global [supersymmetry](../../../../../supersymmetry-split.md) limit $\kappa\to0$, the [F-term scalar potential](../../../../../f-term-scalar-potential.md) becomes $|\lambda|^2(ab+ac+bc)$ and the [D-term scalar potential](../../../../../d-term-scalar-potential.md) retains its form. The same two types of branches occur, with the threshold $|\lambda|^2a>2g|\zeta|$. [Supergravity](../../../../../supergravity.md) instead introduces the exponential and additional positive terms. The [goldstino](../../../../../goldstino.md) of global [supersymmetry breaking](../../../../../supersymmetry-breaking.md) is a physical [fermion](../../../../../fermion.md); in local [supersymmetry](../../../../../supersymmetry-split.md) it participates in the [super-Higgs mechanism](../../../../../super-higgs-mechanism.md). A positive vacuum energy also gravitates in [supergravity](../../../../../supergravity.md). In particular, the positive-energy branch here has $W=0$ and hence vanishing [gravitino mass from a superpotential](../../../../../gravitino-mass-from-a-superpotential.md); it is not the tuned zero-energy broken vacuum of Question 3.

There is a further gauge-consistency qualification. In conventional two-derivative matter-coupled [supergravity](../../../../../supergravity.md), a constant [Fayet–Iliopoulos term](../../../../../fayet-iliopoulos-term.md) gauges an [R-symmetry](../../../../../r-symmetry.md) and requires a corresponding nontrivial transformation of the [superpotential](../../../../../superpotential.md). The apparent charges $0,+1,-1$ make the supplied cubic [superpotential](../../../../../superpotential.md) neutral, so a nonzero independent constant $\zeta$ does not by itself specify a consistent conventional [supergravity](../../../../../supergravity.md) action. The computed branches are those of the supplied [scalar potential](../../../../../scalar-potential.md); a full embedding needs compatible charges or additional fields. This restriction is explained in [Van Proeyen's derivation of the superpotential gauge-covariance condition](https://arxiv.org/abs/hep-th/0410053).

More generally, the [supergravity moment-map constraint on D-term breaking](../../../../../supergravity-moment-map-constraint-on-d-term-breaking.md) follows directly from gauge covariance. If $k^i\partial_iW=-\kappa^2rW$ and the [moment map](../../../../../moment-map.md) is $\mathcal P=i(k^iK_i-r)$, then at a point with $W\ne0$,

$$
\mathcal P=i\kappa^{-2}\frac{k^iD_iW}{W}.
$$

Consequently all chiral [auxiliary fields](../../../../../auxiliary-field.md) vanishing implies the [D-term](../../../../../d-term.md) also vanishes there. This relation has no analogue forcing that implication in an arbitrary global [supersymmetry](../../../../../supersymmetry-split.md) model. Its $W\ne0$ hypothesis matters: the formal D-breaking branch above has $W=0$, so it does not contradict the identity. These conventional gauge-completion restrictions are additional to the elementary minimization calculation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
