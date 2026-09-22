<h1 id="21h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $u=e^{2\pi i y}$ and $w=e^{2\pi i z}$, define

$$
\Phi:M\longrightarrow N,
\qquad
\Phi([t,(u,w)])=\Gamma v(-t,y,z).
$$

Changing $y$ or $z$ by an integer changes $v(-t,y,z)$ by left multiplication by an element of $\Gamma$, so $\Phi$ is independent of the chosen lifts. It also respects the mapping-torus seam because

$$
v(1,0,0)v(-1,y,z)=v(0,y+z,z),
$$

which is exactly the identification

$$
(1,(u,w))\sim(0,(uw,w))=(0,f(u,w)).
$$

Every $\Gamma$-orbit has a representative with its first coordinate in $[-1,0]$, so $\Phi$ is surjective. If two such representatives lie in one orbit, the integer shift of their first coordinates is zero unless they are opposite endpoints; in the first case their torus coordinates agree, and in the endpoint case they are related by the displayed seam. Thus $\Phi$ is injective. It is continuous, $M$ is compact, and $N$ is Hausdorff, so a continuous-bijection theorem gives

$$
\boxed{\ M\cong N.\ }
$$

This realizes the [Heisenberg nilmanifold as a torus mapping torus](../../../../../../heisenberg-nilmanifold-as-a-torus-mapping-torus.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [21H](../../21h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
