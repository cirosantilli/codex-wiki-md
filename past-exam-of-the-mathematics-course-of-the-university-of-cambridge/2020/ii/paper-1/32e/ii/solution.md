<h1 id="32e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $a<0$. Near the pitchfork at $(\mu,x)=(a,0)$, put $\lambda=\mu-a$. Keeping the lowest terms that distinguish the branches gives

$$
\dot x=-2a\,x(\lambda-x^2)+\text{higher-order terms}.
$$

Since $-2a>0$, this is the [pitchfork bifurcation normal form](../../../../../../pitchfork-bifurcation-normal-form.md): the zero branch changes from stable to unstable and the stable branches $x=\pm\sqrt\lambda$ appear for $\lambda>0$.

Near $(\mu,x)=(0,0)$, put $\lambda=\mu$. Then

$$
\dot x=-a\,x(x^2-2\lambda)+\text{higher-order terms}.
$$

Here $-a>0$, so for $\lambda>0$ the zero branch is stable and the two nearby nonzero branches are unstable. This confirms the parameter-reversed [subcritical pitchfork bifurcation](../../../../../../subcritical-pitchfork-bifurcation.md).

Finally fix either $x_0=\pm\sqrt{-2a}$ and put

$$
\mu=-a+m,qquad x=x_0+u.
$$

The two vanishing factors have the leading expansions

$$
x^2-2\mu=2x_0u-2m+O(u^2),qquad
x^2-\mu+a=2x_0u-m+O(u^2).
$$

With the parameter-dependent coordinate $w=2x_0u-m$,

$$
\dot w=2x_0\dot u
=-2x_0^2w(w-m)+\text{higher-order terms}
=2x_0^2w(m-w)+\cdots.
$$

This is the [transcritical bifurcation](../../../../../../transcritical-bifurcation.md) normal form: the branches $w=0$ and $w=m$ cross and exchange stability.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [32E](../../32e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
