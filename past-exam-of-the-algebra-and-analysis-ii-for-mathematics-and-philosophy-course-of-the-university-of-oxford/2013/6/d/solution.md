<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

It suffices to construct an [injective](../../../../injective-function.md) [holomorphic](../../../../holomorphic-function-split.md) map $\Phi_j:U_j\to\mathbb D$ for each domain. Then $\Phi_j\circ f$ is a [bounded](../../../../boundedness.md) [entire function](../../../../entire-function.md) and is constant by [Liouville's theorem](../../../../liouville-theorem.md); [injectivity](../../../../injective-function.md) of $\Phi_j$ forces $f$ to be constant.

For the [upper half-plane](../../../../upper-half-plane-complex-analysis.md), use the [Cayley transform between the half-plane and disk](../../../../cayley-transform-between-the-half-plane-and-disk.md)

$$
\Phi_1(z)=\frac{z-i}{z+i}.
$$

Its denominator is nonzero there, and $|z+i|^2-|z-i|^2=4\operatorname{Im}z>0$, so its [image](../../../../image-of-a-function.md) lies in the [unit disk](../../../../unit-disk.md). The [determinant](../../../../determinant.md) is nonzero, hence it is [injective](../../../../injective-function.md) and [conformal](../../../../conformal-map.md).

On the plane slit along the nonnegative real axis, choose the branch

$$
S(z)=\sqrt{|z|}\,e^{i\operatorname{Arg}z/2},\qquad0<\operatorname{Arg}z<2\pi.
$$

This is the [holomorphic square root](../../../../holomorphic-square-root.md) obtained from the corresponding [logarithm branch](../../../../branch-of-the-complex-logarithm.md). Its [argument](../../../../argument-complex-analysis.md) lies in $(0,\pi)$, so it maps $U_2$ bijectively onto the [upper half-plane](../../../../upper-half-plane-complex-analysis.md), with inverse $w\mapsto w^2$. Its [derivative](../../../../derivative.md) is $1/(2S(z))\neq0$. Therefore

$$
\Phi_2(z)=\frac{S(z)-i}{S(z)+i}
$$

is an [injective](../../../../injective-function.md) [conformal map](../../../../conformal-map.md) of $U_2$ onto the [unit disk](../../../../unit-disk.md).

For the complement of the closed interval, first use

$$
M(z)=\frac{z}{1-z}.
$$

Its only finite pole is the excluded point one, and it is [injective](../../../../injective-function.md) with [derivative](../../../../derivative.md) $1/(1-z)^2\neq0$. If $M(z)=t\geq0$, solving gives $z=t/(1+t)\in[0,1)$, which is excluded. Hence $M(U_3)\subset U_2$, and

$$
\Phi_3(z)=\Phi_2\left(\frac{z}{1-z}\right)
$$

is the required [injective](../../../../injective-function.md) [conformal map](../../../../conformal-map.md) into the disk. More precisely, $M(U_3)=U_2\setminus\{-1\}$ and $\Phi_3(U_3)=\mathbb D\setminus\{0\}$, since $S(-1)=i$. No claim that the interval complement is conformally equivalent to the whole disk is required.

Applying Liouville to the three [bounded](../../../../boundedness.md) compositions gives

$$
\boxed{f:\mathbb C\to U_j\text{ holomorphic}\Longrightarrow f\text{ constant},\qquad j=1,2,3.}
$$

This illustrates [Liouville rigidity from a bounded holomorphic embedding](../../../../liouville-rigidity-from-a-bounded-holomorphic-embedding.md): an explicit [injective](../../../../injective-function.md) [bounded](../../../../boundedness.md) coordinate is enough.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../split.md)
5. [Algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../../algebra-and-analysis-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Mathematics and philosophy course of the University of Oxford](../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
