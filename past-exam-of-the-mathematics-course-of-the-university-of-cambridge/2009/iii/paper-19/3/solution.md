<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [irreducible complex analytic hypersurface](../../../../../complex-analytic-hypersurface.md) is a closed analytic subset of pure complex codimension one which cannot be expressed as the union of two proper closed analytic subsets. Here a [local defining function of a complex analytic hypersurface](../../../../../local-defining-function-of-a-complex-analytic-hypersurface.md) means a reduced local equation: a [holomorphic](../../../../../complex-differentiability-at-a-point.md) germ generating its vanishing ideal, with each local branch occurring once. The word reduced matters. Merely prescribing the zero set would allow both $f$ and $f^2$, and the requested uniqueness would then be false.

The local facts used are these: in [holomorphic coordinates](../../../../../holomorphic-coordinate.md) the [local ring](../../../../../local-ring.md) $\mathcal O_{X,p}$ is $\mathbb C\{z_1,\ldots,z_n\}$, a [regular local ring](../../../../../regular-local-ring.md) and a [unique factorization domain](../../../../../unique-factorization-domain.md); its units are exactly the germs nonzero at $p$; and the analytic Nullstellensatz identifies the zero-set ideal of a germ $f$ with $\sqrt{(f)}$. A reduced germ is a product of distinct irreducible factors. [Unique factorization](../../../../../unique-factorization-in-an-integral-domain.md) makes its [principal ideal](../../../../../principal-ideal.md) radical: if $f\mid h^r$, every irreducible factor of $f$ divides $h$, so $f\mid h$. Thus two reduced germs with the same hypersurface germ have $(f)=(g)$. Write $g=uf$, $f=vg$. The [local ring](../../../../../local-ring.md) is a domain, so $uv=1$. Hence $u$ is a [holomorphic](../../../../../complex-differentiability-at-a-point.md) unit and $u(p)\ne0$. This proves [reduced local defining functions differ by a holomorphic unit](../../../../../reduced-local-defining-functions-differ-by-a-holomorphic-unit.md). Global irreducibility does not imply local irreducibility at a singular point; the same argument uses the product of all local branches and therefore covers that case too.

A [divisor on a complex manifold](../../../../../divisor-on-a-complex-manifold.md) is a locally finite integer combination of irreducible analytic hypersurfaces. On a [compact](../../../../../compact-space.md) manifold only finitely many have nonzero coefficients. Choose local meromorphic equations $f_i$ for a divisor $D$, by products of powers of reduced local equations. Their ratios are [holomorphic](../../../../../complex-differentiability-at-a-point.md) units on overlaps. For the [holomorphic line bundle associated to a divisor](../../../../../holomorphic-line-bundle-associated-to-a-divisor.md), choose frames satisfying

$$
e_i=\frac{f_j}{f_i}e_j.
$$

The ratios obey the cocycle identity and so define a [holomorphic line bundle](../../../../../holomorphic-line-bundle.md) $[D]$. This convention makes the local meromorphic sections $f_i e_i$ agree, with divisor $D$. Changing the equations by units changes frames and gives an isomorphic bundle.

For hyperplanes $H_1,H_2$ in [Complex projective space](../../../../../complex-projective-space.md), choose nonzero linear equations $\ell_1,\ell_2$. The degree-zero quotient $r=\ell_1/\ell_2$ is a global [meromorphic function](../../../../../meromorphic-function.md) and has divisor $H_1-H_2$. A [principal divisor on a complex manifold](../../../../../principal-divisor-on-a-complex-manifold.md) gives a trivial associated bundle: using the same global meromorphic equation on every chart makes all frame transitions equal to one. The allowed tensor-product rule now gives

$$
[H_1]\otimes[H_2]^{-1}\cong[H_1-H_2]\cong\mathcal O,
\qquad\boxed{[H_1]\cong[H_2].}
$$

If the hyperplanes coincide the same conclusion is immediate. Equivalently, their common bundle is the hyperplane bundle $\mathcal O(1)$.

Locally at the centre of a [blowup of a complex manifold at a point](../../../../../blowup-of-a-complex-manifold-at-a-point.md), replace a coordinate neighbourhood in $\mathbb C^n$ by

$$
\widetilde U=\{(z,[\ell])\in U\times\mathbb{CP}^{n-1}:z_i\ell_j=z_j\ell_i\text{ for all }i,j\},
\qquad\sigma(z,[\ell])=z.
$$

Away from zero the direction is uniquely $[z]$, so this map is an isomorphism there; glue it to $X\setminus\{p\}$. In the chart $\ell_j\ne0$, write $z_j=u$ and $z_i=ut_i$ for $i\ne j$. These are smooth [holomorphic coordinates](../../../../../holomorphic-coordinate.md) on the blowup. The [exceptional divisor](../../../../../exceptional-divisor.md) is $u=0$, globally $E=\sigma^{-1}(p)\cong\mathbb P(T_pX)$.

The [canonical bundle formula for a point blowup](../../../../../canonical-bundle-formula-for-a-point-blowup.md) is

$$
\boxed{K_{\widetilde X}\cong\sigma^*K_X\otimes[E]^{\otimes(n-1)}.}
$$

The local chart also explains the exponent: pulling back a coordinate volume form gives $\pm u^{n-1}du\wedge\bigwedge_{i\ne j}dt_i$, so the Jacobian section has divisor $(n-1)E$.

Since $Y$ is smooth at the centre, choose coordinates with $Y=\{z_1=0\}$. Its [strict transform](../../../../../strict-transform.md) is a genuine analytic hypersurface. In a blowup chart $j\ne1$, it is the closed set $t_1=0$: off $E$, the original equation $ut_1=0$ reduces to $t_1=0$, and taking the closure restores the points with $u=0$. In chart $j=1$, there are no such off-exceptional points, and the [strict transform](../../../../../strict-transform.md) is empty there. These descriptions agree on overlaps and show analyticity, with $\widetilde Y\cap E\cong\mathbb{CP}^{n-2}$. The total transform has the extra factor $u$ exactly once, so

$$
\sigma^*Y=\widetilde Y+E,
\qquad[-\widetilde Y]\cong\sigma^*[-Y]\otimes[E].
$$

Under the given anticanonical assumption, this yields

$$
\boxed{[-\widetilde Y]\cong K_{\widetilde X}\otimes[E]^{\otimes(2-n)}.}
$$

To prove the only-if direction, one must rule out an accidental trivial power of $[E]$. The local blowup is the tautological [line bundle](../../../../../line-bundle.md) over $\mathbb{CP}^{n-1}$, with $E$ its zero section. Its [normal bundle](../../../../../normal-bundle.md) is therefore $\mathcal O_E(-1)$. The [normal bundle of a smooth analytic hypersurface](../../../../../normal-bundle-of-a-smooth-analytic-hypersurface.md) identifies $[E]|_E$ with this bundle. If $n\ge2$, restrict to a [projective line](../../../../../projective-line.md) inside $E$; the restriction of $[E]^{\otimes(2-n)}$ has degree $n-2$. A trivial [line bundle](../../../../../line-bundle.md) has degree zero, so it is trivial only if $n=2$. Conversely the displayed tensor factor is literally trivial when $n=2$. This is the [anticanonical strict transform under a point blowup](../../../../../anticanonical-strict-transform-under-a-point-blowup.md) criterion:

$$
\boxed{[-\widetilde Y]\cong K_{\widetilde X}\ \Longleftrightarrow\ n=2.}
$$

For completeness, dimension one cannot satisfy the premise in this [compact](../../../../../compact-space.md) setting: an irreducible analytic hypersurface is one point, and $[-Y]$ has degree $-1$ on its curve component, whereas $K_X$ has degree $2g-2$. Thus no exceptional dimension-one case invalidates the equivalence.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
