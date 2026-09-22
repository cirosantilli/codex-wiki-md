<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For fixed-endpoint variations, the [second variation](../../../../second-variation.md) is

$$
q(\varphi)=\delta^2I(\bar u)(\varphi,\varphi)=\left.\frac{d^2}{dt^2}I(\bar u+t\varphi)\right|_{t=0}=\int_a^b(p\varphi'^2+2r\varphi\varphi'+s\varphi^2)dx,
$$

with $p=f_{vv}$, $r=f_{uv}$, $s=f_{uu}$ evaluated along $(x,\bar u,\bar u')$. The [Jacobi equation](../../../../jacobi-equation.md), written without differentiating $r$ separately, is

$$
\boxed{-(pz'+rz)'+rz'+sz=0.}
$$

When $r$ is differentiable this is $-(pz')'+(s-r')z=0$.

[Positive definiteness](../../../../positive-definiteness.md) means $q(\varphi)>0$ for every nonzero admissible variation. Uniform or [coercive positivity of a second variation](../../../../coercive-positivity-of-a-second-variation.md) is the stronger assertion that $q(\varphi)\geq c\int\varphi'^2$ for some fixed $c>0$. On a fixed-endpoint interval this is equivalent to a positive lower bound in the $W^{1,2}$ norm.

**The strict Legendre implication uses the uniform interpretation of positivity.** If $q\geq c\int\varphi'^2$, localized rapidly oscillating variations show $p(x)\geq c$: otherwise support them in an interval where $p-c<0$, so the [derivative](../../../../derivative.md) term of $q-c\int\varphi'^2$ is negative of order frequency squared, overwhelming its mixed and zero-order terms. Continuity extends the bound to the endpoints, giving $p>0$ on $[a,b]$. Under mere [positive definiteness](../../../../positive-definiteness.md) this strict conclusion is false: $f=u^2$ at $\bar u=0$ gives $q=2\int\varphi^2>0$ but $p=0$. In that weaker convention only the ordinary [Legendre necessary condition](../../../../legendre-necessary-condition.md) $p\geq0$ follows. This distinction makes the implication precise.

Under the stated regular condition $p>0$, a [conjugate point](../../../../conjugate-point.md) $c\in(a,b]$ to $a$ is an endpoint admitting a nonzero Jacobi solution with $z(a)=z(c)=0$. The disconjugacy form of the [Jacobi positivity criterion](../../../../jacobi-positivity-criterion.md) says that no such point in $(a,b]$ exists if and only if there is a Jacobi solution strictly positive on all of $[a,b]$.

For the required identity, let that positive solution be $z$ and write $\varphi=zh$. Set $A=pzz'+rz^2$. The [Jacobi equation](../../../../jacobi-equation.md) gives

$$
A'=pz'^2+2rzz'+sz^2.
$$

Expanding the second-variation integrand therefore yields

$$
p\varphi'^2+2r\varphi\varphi'+s\varphi^2=pz^2h'^2+(Ah^2)'.
$$

For compactly supported $\varphi$, the [boundary term](../../../../boundary-term.md) vanishes, proving

$$
\boxed{\delta^2I(\bar u)(\varphi,\varphi)=\int_a^bpz^2\left[\left(\frac\varphi z\right)'\right]^2dx.}
$$

This is the [Jacobi identity for the second variation](../../../../jacobi-identity-for-the-second-variation.md). The divergence form is also appropriate under the original $C^1$ regularity; with $p>0$, the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) gives the usual further regularity along the extremal.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the calculus of variations course of the University of Oxford](../../../split.md)
5. [Calculus of variations course of the University of Oxford](../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
