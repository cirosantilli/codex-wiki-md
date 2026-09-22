<h1 id="7a/solution">Solution</h1>

↑ **Parent:** [7A](../7a.md)

With consistent flux and loop orientations, [Faraday's law](../../../../../faraday-s-law-of-induction.md) is $V=-d\Phi/dt$. The [magnetic force on a current-carrying wire](../../../../../magnetic-force-on-a-current-carrying-wire.md) is $d\mathbf F=I\,d\boldsymbol\ell\times\mathbf B$.

Let $z(t)$ be the top edge height and $v=-\dot z$ the downward speed. While $0<z<l$, only the top horizontal edge lies in the field, and the linked [magnetic flux](../../../../../magnetic-flux.md) is $Bwz$. Therefore the induced [electromotive force](../../../../../electromotive-force.md) has magnitude $Bwv$, and [Ohm's law](../../../../../ohm-s-law.md) gives current magnitude $I=Bwv/R$. Its force opposes the downward motion and has upward magnitude $IBw=B^2w^2v/R$. Forces on the vertical sides cancel horizontally. Hence

$$
\boxed{m\dot v=mg-\frac{B^2w^2}{R}v,\qquad
m\ddot z=-mg-\frac{B^2w^2}{R}\dot z,\qquad
v_{\rm terminal}=\frac{mgR}{B^2w^2}.}
$$

For a release from rest, $v=v_{\rm terminal}(1-e^{-B^2w^2t/(mR)})$. The terminal speed is the formal limit while partial overlap is maintained; after the entire loop leaves the field this magnetic braking term vanishes.

## ↑ Ancestors (10)

1. [7A](../7a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
