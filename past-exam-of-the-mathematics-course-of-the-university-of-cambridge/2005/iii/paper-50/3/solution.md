<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Adjoint representation of a Lie algebra](../../../../../adjoint-representation-of-a-lie-algebra.md) acts on the [Lie algebra](../../../../../lie-algebra-split.md) itself by $\operatorname{ad}_X(Y)=[X,Y]$. The [Jacobi identity](../../../../../jacobi-identity.md) gives

$$
[\operatorname{ad}_X,\operatorname{ad}_Y]Z=[X,[Y,Z]]-[Y,[X,Z]]=[[X,Y],Z]=\operatorname{ad}_{[X,Y]}Z.
$$

Thus it is a [Lie algebra representation](../../../../../lie-algebra-representation.md). In the basis $T_a$ with $[T_a,T_b]=c^c{}_{ab}T_c$, its matrices are

$$
\boxed{(T_a^{\rm ad})^c{}_b=c^c{}_{ab},\qquad[T_a^{\rm ad},T_b^{\rm ad}]=c^c{}_{ab}T_c^{\rm ad}.}
$$

The column index labels the basis vector being acted on; this convention fixes the matrix signs.

Work in finite dimension over characteristic zero, as in the usual real or complex gauge algebras. A [simple Lie algebra](../../../../../simple-lie-algebra.md) is nonabelian and has no nonzero proper [Lie algebra ideal](../../../../../ideal-of-a-lie-algebra.md). A [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) has no nonzero solvable ideal; equivalently it is a direct sum of simple ideals. The nondegenerate [Killing form](../../../../../killing-form.md) is $\kappa(X,Y)=\operatorname{tr}(\operatorname{ad}_X\operatorname{ad}_Y)$. Its invariance follows from the representation identity and trace cyclicity:

$$
\kappa([X,Y],Z)=\operatorname{tr}([\operatorname{ad}_X,\operatorname{ad}_Y]\operatorname{ad}_Z)=\kappa(X,[Y,Z]).
$$

For the reduction, take a nonzero proper ideal $\mathfrak a$, if one exists, and define its Killing-orthogonal complement $\mathfrak a^\perp$. Invariance makes it an ideal: for $y\in\mathfrak a^\perp$, $x\in L$, $z\in\mathfrak a$, $\kappa([x,y],z)=-\kappa(y,[x,z])=0$. Moreover $[\mathfrak a,\mathfrak a^\perp]=0$, because for $u\in\mathfrak a$, $v\in\mathfrak a^\perp$, and any $x\in L$,

$$
\kappa([u,v],x)=\kappa(v,[x,u])=0,
$$

and the global [Killing form](../../../../../killing-form.md) is nondegenerate. Their intersection is consequently an abelian ideal: its elements lie in both commuting ideals. Semisimplicity forces that intersection to be zero. The dimension formula for a nondegenerate bilinear form then gives

$$
L=\mathfrak a\oplus\mathfrak a^\perp.
$$

The summands commute and are semisimple, since a solvable ideal in either summand would also be an ideal of $L$. Repeating on smaller summands terminates in simple ideals. This proves the [orthogonal ideal splitting for a nondegenerate Killing form](../../../../../orthogonal-ideal-splitting-for-a-nondegenerate-killing-form.md) and describes the required reduction; abelian one-dimensional factors do not occur in a semisimple algebra.

If $\kappa(T_a,T_b)=\ell\delta_{ab}$ with $\ell\ne0$, invariance gives

$$
\kappa([T_a,T_b],T_c)+\kappa(T_b,[T_a,T_c])=0,
$$

so $c_{abc}=-c_{acb}$ after lowering the output index with $\delta$. The bracket already gives $c_{abc}=-c_{bac}$. These two adjacent transpositions generate all permutations, proving that the [structure constants of a Lie algebra](../../../../../structure-constant-of-a-lie-algebra.md) are completely antisymmetric. This is the [antisymmetry of Killing-lowered structure constants](../../../../../antisymmetry-of-killing-lowered-structure-constants.md); the scalar $\ell$ cancels in the chosen normalization.

For the gauge calculation write $\Lambda=\lambda_at_a$, $A_\mu=A_{\mu a}t_a$, and $D_\mu=\partial_\mu+A_\mu$. The representation generators here obey $[t_a,t_b]=c_{abc}t_c$; factors of $i$ and the gauge coupling are absorbed in this connection convention. Expanding the varied derivative gives

$$
\delta(D_\mu\phi)=(\partial_\mu\Lambda)\phi+\Lambda\partial_\mu\phi+(\delta A_\mu)\phi+A_\mu\Lambda\phi.
$$

For this to equal $\Lambda D_\mu\phi$, choose the [gauge transformation in the derivative-plus-connection convention](../../../../../gauge-transformation-in-the-derivative-plus-connection-convention.md)

$$
\boxed{\delta A_\mu=-\partial_\mu\Lambda+[\Lambda,A_\mu],\qquad\delta A_{\mu a}=-\partial_\mu\lambda_a+c_{abc}\lambda_bA_{\mu c}.}
$$

Then all extra terms cancel, proving covariance of the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) for arbitrary space-dependent parameters.

Apply both derivatives to a test field. The second derivatives commute and the terms involving one derivative of the field cancel, leaving the [Yang-Mills field strength](../../../../../gauge-field-strength.md)

$$
[D_\mu,D_\nu]\phi=F_{\mu\nu}\phi,\qquad F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+[A_\mu,A_\nu].
$$

Thus its components are

$$
\boxed{F_{\mu\nu a}=\partial_\mu A_{\nu a}-\partial_\nu A_{\mu a}+c_{abc}A_{\mu b}A_{\nu c}.}
$$

The already obtained variation can be written $\delta D_\mu=[\Lambda,D_\mu]$. The operator [Jacobi identity](../../../../../jacobi-identity.md) then yields

$$
\delta F_{\mu\nu}=[[\Lambda,D_\mu],D_\nu]+[D_\mu,[\Lambda,D_\nu]]=[\Lambda,[D_\mu,D_\nu]]=[\Lambda,F_{\mu\nu}],
$$

or

$$
\boxed{\delta F_{\mu\nu a}=c_{abc}\lambda_bF_{\mu\nu c}.}
$$

Finally, with fixed space-time metric,

$$
\delta\left(-\frac14F^{\mu\nu}_aF_{\mu\nu a}\right)=-\frac12c_{abc}\lambda_bF^{\mu\nu}_aF_{\mu\nu c}=0.
$$

The contracted product is symmetric in $a,c$, while $c_{abc}$ is antisymmetric in those indices. Hence the [Yang-Mills action](../../../../../yang-mills-action.md) density is gauge invariant, with the sign convention derived rather than assumed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
