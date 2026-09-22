<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $g_2=60G_4$ and $g_3=140G_6$, with the lattice sums taken over nonzero lattice elements. Reindexing the normally convergent series shows that the [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) $\wp$ is an [even function](../../../../../even-function.md), and consequently $\wp'$ is an [odd function](../../../../../odd-function.md). Expanding $(z-w)^{-2}$ near zero and cancelling the odd lattice sums gives the [Laurent coefficients of the Weierstrass elliptic function](../../../../../laurent-coefficients-of-the-weierstrass-elliptic-function.md)

$$
\wp(z)=z^{-2}+3G_4z^2+5G_6z^4+O(z^6),\qquad
\wp'(z)=-2z^{-3}+6G_4z+20G_6z^3+O(z^5).
$$

Thus the [elliptic function](../../../../../elliptic-function.md) $\wp'^2-4\wp^3+60G_4\wp$ has no pole at zero and its constant term is $-140G_6$. By periodicity it has no poles anywhere. An entire [elliptic function](../../../../../elliptic-function.md) is bounded on a fundamental parallelogram and hence everywhere, so [Liouville theorem](../../../../../liouville-theorem.md) makes it constant. This proves the [Weierstrass elliptic differential equation](../../../../../weierstrass-elliptic-differential-equation.md)

$$
\boxed{\wp'^2=4\wp^3-g_2\wp-g_3.}
$$

We first verify that the cubic is smooth, rather than presupposing it when using its group law. There are three nonzero [two-torsion points of a complex torus](../../../../../two-torsion-point-of-a-complex-torus.md) $h_j\in(\tfrac12\Lambda)/\Lambda$. Oddness and periodicity imply $\wp'(h_j)=0$. Since $\wp'$ has a triple pole and no other poles on the torus, [value multiplicity of an elliptic function](../../../../../value-multiplicity-of-an-elliptic-function.md) says that these three distinct zeros exhaust its zeros and are simple. Put $e_j=\wp(h_j)$. Each $\wp-e_j$ has a double zero at $h_j$, since $\wp'(h_j)=0$ and the zero of $\wp'$ is simple. If $e_i=e_j$ with $i\ne j$, this same function would have at least four zeros counted with [multiplicity](../../../../../multiplicity-mathematics.md), although its only pole is double. Therefore the [half-period values of the Weierstrass elliptic function](../../../../../half-period-values-of-the-weierstrass-elliptic-function.md) are distinct. They are roots of $4x^3-g_2x-g_3$, so all its roots are distinct and the affine curve is a [smooth algebraic curve](../../../../../smooth-algebraic-curve.md). Its [projective closure](../../../../../projective-completion.md) is

$$
Y^2Z=4X^3-g_2XZ^2-g_3Z^3.
$$

It has the single point $O=(0:1:0)$ at infinity. The derivative with respect to $Z$ of the defining homogeneous polynomial is nonzero at $O$, proving smoothness there too.

For any finite value $a$, [value multiplicity of an elliptic function](../../../../../value-multiplicity-of-an-elliptic-function.md) gives exactly two solutions of $\wp(z)=a$, counting [multiplicities](../../../../../multiplicity-mathematics.md). Evenness supplies the pair $z,-z$. At a nonzero half-period these coincide and the zero is double; elsewhere they are distinct. An even [elliptic function](../../../../../elliptic-function.md) $f$ therefore descends to a meromorphic function of $x=\wp(z)$ on the [Riemann sphere](../../../../../riemann-sphere.md). To justify descent at a half-period, put $z=h+u$: both $f(h+u)$ and $\wp(h+u)$ are even in $u$, and $\wp(h+u)-\wp(h)$ is $u^2$ times a nonvanishing even analytic function. The local [Laurent series](../../../../../laurent-series.md) of $f$ is consequently meromorphic in the coordinate $x-e$. At zero the same argument uses $1/x=z^2+O(z^6)$. Every [meromorphic function](../../../../../meromorphic-function.md) on the [Riemann sphere](../../../../../riemann-sphere.md) is a [rational function](../../../../../rational-function.md), proving that [even elliptic functions are rational in the Weierstrass function](../../../../../even-elliptic-functions-are-rational-in-the-weierstrass-function.md).

For an arbitrary [elliptic function](../../../../../elliptic-function.md) $f$, its even part $(f(z)+f(-z))/2$ is $A(\wp)$. Its odd part divided by $\wp'$ is an even [meromorphic function](../../../../../meromorphic-function.md), hence is $B(\wp)$ with $B$ rational. We have therefore proved the [elliptic function-field decomposition](../../../../../elliptic-function-field-decomposition.md)

$$
\boxed{f(z)=A(\wp(z))+\wp'(z)B(\wp(z)),\qquad A,B\in\mathbb C(x).}
$$

Uniqueness follows by taking even and odd parts. In particular the field of [elliptic functions](../../../../../elliptic-function.md) is $\mathbb C(\wp,\wp')$.

Define $\Phi(0)=O$ and $\Phi(z)=(\wp(z),\wp'(z))$ elsewhere on $\mathbb C/\Lambda$. Periodicity makes the map well defined. Near zero, the projective chart $Y\ne0$ has coordinates $X/Y=\wp/\wp'=-z/2+O(z^5)$ and $Z/Y=1/\wp'=-z^3/2+O(z^7)$, so the extension is holomorphic. The fiber description above proves injectivity: the two candidates $z,-z$ are distinguished by $\wp'$ unless they coincide at a half-period. It also proves surjectivity, since every $x$ occurs and the two derivatives are the two allowed $y$ values, with $y=0$ at a branch value.

Finally, a nonvertical line $y=ax+b$ pulls back to the [elliptic function](../../../../../elliptic-function.md) $\wp'-a\wp-b$, whose only pole is triple at zero. Its three zeros $z_1,z_2,z_3$, counted with [intersection multiplicity](../../../../../intersection-multiplicity.md), satisfy $z_1+z_2+z_3=0$ modulo $\Lambda$ by the [zero-pole sum of an elliptic function](../../../../../zero-pole-sum-of-an-elliptic-function.md). On the cubic, reflection $y\mapsto-y$ corresponds to $z\mapsto-z$. The [chord-and-tangent group law](../../../../../chord-and-tangent-group-law.md) therefore gives $\Phi(z_1)+\Phi(z_2)=\Phi(-z_3)=\Phi(z_1+z_2)$. Vertical lines give inverse pairs; tangencies are included through repeated zeros, and the identity cases follow from the extension at zero. This completes the [Weierstrass uniformization by half-period values](../../../../../weierstrass-uniformization-by-half-period-values.md): **$\Phi$ is a group isomorphism.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
