<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose the [shock wave](../../../../../../../shock-wave.md) normal to point from $S<0$ to $S>0$:

$$
\mathbf n=\frac{\nabla S}{|\nabla S|},\qquad v_n=\mathbf v\cdot\mathbf n=-\frac{S_t}{|\nabla S|}.
$$

The latter identity follows by differentiating $S(\mathbf x_s(t),t)=0$ along the moving surface. Write $[a]=a^+-a^-$ and $[\mathbf b]=\mathbf b^+-\mathbf b^-$. The [distributional derivative of the Heaviside step function](../../../../../../../distributional-derivative-of-the-heaviside-step-function.md) is $\partial_tH(S)=S_t\delta(S)$ and $\nabla H(S)=\nabla S\,\delta(S)$. The regular terms cancel using the conservation equations on each side, leaving

$$
\partial_ta+\nabla\cdot\mathbf b=\left([a]S_t+[\mathbf b]\cdot\nabla S\right)\delta(S)=\left([\mathbf b]-\mathbf v[a]\right)\cdot\mathbf n\,|\nabla S|\delta(S).
$$

Thus the explicitly requested vector is

$$
\boxed{\mathbf f=[\mathbf b]-\mathbf v[a].}
$$

Only its normal component matters; adding tangential velocity to the surface parametrization changes neither result. The invariant [surface delta distribution](../../../../../../../surface-delta-distribution.md) is $\delta_s=|\nabla S|\delta(S)$, so the formula is the [moving-interface conservation jump identity](../../../../../../../moving-interface-conservation-jump-identity.md) $\partial_ta+\nabla\cdot\mathbf b=([\mathbf b]\cdot\mathbf n-v_n[a])\delta_s$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 77](../../../../paper-77-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
