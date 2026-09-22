<h1 id="1/iii/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $X(t)$ be the advancing nose into previously unoccupied pores. In the advective limit the interior flux is $uh$, while the exterior current thickness and flux are zero. Applying the [Rankine-Hugoniot condition](../../../../../../../rankine-hugoniot-conditions.md) to the storage $\phi h$ gives

$$
\boxed{\phi\dot X=u,\qquad X(0)=0,\qquad X(t)=\frac{ut}{\phi}.}
$$

This is the leading-edge kinematic boundary condition. The outer depth immediately behind this nose is $h(X(t)^-,t)=h_0$, whereas ahead it is zero. A first-order [advection](../../../../../../../advection.md) model allows this jump; imposing zero depth on its interior trace would contradict its characteristic solution.

For the full [inclined porous gravity current](../../../../../../../inclined-porous-gravity-current.md), the nose is instead resolved by a continuous spreading layer with $h(X,t)=0$. Taking the flux divided by depth at that interface gives $\dot X=(u/\phi)(1-\cot\theta\,h_x|_{X^-})$, when this one-sided derivative exists. Its leading outer value is $u/\phi$ only when the nose correction is negligible on the scale of the approximation. The zero-depth condition belongs to that resolved layer, not to the discontinuous outer profile itself.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Iii](../../iii.md)
3. [1](../../../1.md)
4. [Paper 73](../../../../paper-73-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
