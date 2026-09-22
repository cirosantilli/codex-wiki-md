<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Using the printed convention that the projective points represent lines of [binary quartics](../../../../../binary-quartic.md), the locus of [GIT stable points](../../../../../stable-projective-point-in-geometric-invariant-theory.md) is

$$
\boxed{\{[f]:f\text{ has four distinct roots in }\mathbb P^1\}
=\{[f]:\operatorname{Disc}(f)\ne0\}.}
$$

The root at infinity is included. We determine stability by calculating every relevant [algebraic one-parameter subgroup](../../../../../algebraic-one-parameter-subgroup.md) weight.

Use the natural action $(g\cdot f)(X,Y)=f(g^{-1}(X,Y))$. Every nontrivial [algebraic one-parameter subgroup](../../../../../algebraic-one-parameter-subgroup.md) of $SL_2$ is conjugate to $\lambda_m(t)=\operatorname{diag}(t^m,t^{-m})$ for some integer $m>0$: its two integral [weights of a representation](../../../../../weight-of-a-representation.md) sum to zero, and a basis of [weight vectors](../../../../../weight-vector.md) can be rescaled to have determinant one. Write

$$
f(X,Y)=\sum_{j=0}^4a_jX^{4-j}Y^j,\qquad
\lambda_m(t)\cdot X^{4-j}Y^j=t^{m(2j-4)}X^{4-j}Y^j.
$$

If $r=\min\{j:a_j\ne0\}$, then $r$ is the [multiplicity of a root](../../../../../multiplicity-of-a-root.md) at the projective point $[1:0]$: in the local coordinate $Y/X$, the [polynomial](../../../../../polynomial-split.md) begins with a nonzero multiple of $(Y/X)^r$.

The [Hilbert-Mumford criterion for projective stability](../../../../../hilbert-mumford-criterion-for-projective-stability.md), with $\mu=-\min$(active weights), now gives

$$
\mu([f],\lambda_m)=m(4-2r).
$$

Being a [GIT stable point](../../../../../stable-projective-point-in-geometric-invariant-theory.md) requires this number to be strictly positive for every nontrivial subgroup. Conjugating the subgroup lets $[1:0]$ range over the entire [projective line](../../../../../projective-line.md). Thus the [root-multiplicity criterion for stable binary forms](../../../../../root-multiplicity-criterion-for-stable-binary-forms.md) becomes $r_p(f)<2$ at every point $p$. A nonzero degree-four form over $\mathbb C$ has four projective roots counted with multiplicity, so this means precisely four distinct roots. This is equivalently nonvanishing of its [discriminant](../../../../../discriminant.md).

The boundary cases show why a weak inequality would give the wrong answer. A triple or quadruple root can be moved to $[1:0]$, leaving only strictly positive weights; its affine representative tends to zero under that subgroup, so it is unstable. If all root multiplicities are at most two, all Hilbert-Mumford values are nonnegative and the point is a [GIT semistable point](../../../../../semistable-projective-point-in-geometric-invariant-theory.md). A double root gives a zero value for a suitable subgroup, so never represents a [GIT stable point](../../../../../stable-projective-point-in-geometric-invariant-theory.md). More concretely, after putting that double root at $[1:0]$ one has

$$
f=Y^2(aX^2+bXY+cY^2),\qquad a\ne0,
$$

and $\lambda_1(t)\cdot f\to aX^2Y^2$. When there are three distinct roots, this limiting form, representing a [GIT semistable point](../../../../../semistable-projective-point-in-geometric-invariant-theory.md) with two distinct roots, is outside the original [group orbit](../../../../../orbit-of-a-group-action.md), so that [group orbit](../../../../../orbit-of-a-group-action.md) is not closed in the semistable locus. When there are two double roots, a change of coordinates gives $X^2Y^2$, which has the positive-dimensional diagonal torus as [stabilizer](../../../../../stabilizer-subgroup.md). Neither case represents a [GIT stable point](../../../../../stable-projective-point-in-geometric-invariant-theory.md).

For a form with four distinct roots, the projective [stabilizer](../../../../../stabilizer-subgroup.md) is finite: it permutes the four roots, and a [Möbius transformation](../../../../../mobius-transformation.md) fixing three distinct points is the identity. Thus its image in $PGL_2$ injects into the finite [permutation group](../../../../../permutation-group.md) on the roots. The [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) for $SL_2\to PGL_2$ is $\{\pm I\}$, also finite. This agrees with the finite-stabilizer condition in [geometric invariant theory](../../../../../geometric-invariant-theory.md). The weight calculation already supplies the required strict stability condition for every conjugate subgroup.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
