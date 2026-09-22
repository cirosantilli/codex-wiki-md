<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Literally, the printed hypothesis with positive $C$ is impossible for pairs at distance less than one, even when $U$ is constant. Use the corrected [log-Lipschitz modulus](../../../../../../log-lipschitz-modulus.md) $\mu$ from part (e). Local existence for the continuous finite-dimensional [vector field](../../../../../../vector-field.md) follows from the [Peano existence theorem](../../../../../../peano-existence-theorem.md). Boundedness gives $|X(t)-X(s)|\leq\|U\|_\infty|t-s|$. Thus a trajectory cannot escape to infinity in finite time; at a finite endpoint it has a limit, and local existence there extends it. **Solutions exist globally.**

For uniqueness, let $X,Y$ have the same initial point and set $\delta(t)=|X(t)-Y(t)|$. This [absolutely continuous function](../../../../../../absolutely-continuous-function.md) satisfies, almost everywhere,

$$
\delta'(t)\leq C\mu(\delta(t)),\qquad \delta(0)=0.
$$

This is the [Osgood uniqueness criterion](../../../../../../osgood-uniqueness-criterion.md), rather than the usual linear [Gronwall inequality](../../../../../../gronwall-inequality.md), because the velocity need not be [Lipschitz continuous](../../../../../../lipschitz-continuity.md). To see the argument directly, put $w_\varepsilon=\delta+\varepsilon$. As long as $w_\varepsilon\leq1$, monotonicity of $\mu$ gives

$$
w_\varepsilon'\leq Cw_\varepsilon(1-\log w_\varepsilon).
$$

For $z_\varepsilon=1-\log w_\varepsilon$, this becomes $z_\varepsilon'\geq-Cz_\varepsilon$. Integration gives

$$
w_\varepsilon(t)\leq
\exp\left(1-(1-\log\varepsilon)e^{-Ct}\right).
$$

For any fixed finite interval, this upper bound tends uniformly to zero as $\varepsilon\downarrow0$. Taking $\varepsilon$ small prevents a first exit through $w_\varepsilon=1$, so the bound remains valid throughout that interval. Thus $\delta=0$. Backward time has the same proof. **Every initial point has exactly one global trajectory.**

The decisive fact is $\int_0^1dr/\mu(r)=\infty$. For different nearby initial points, the same comparison gives

$$
|X(t)-Y(t)|\leq e^{1-e^{-Ct}}|X(0)-Y(0)|^{e^{-Ct}}
$$

until the separation reaches one. This quantitative continuous dependence makes the flow a homeomorphism, although it need not be a smooth [diffeomorphism](../../../../../../diffeomorphism.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
