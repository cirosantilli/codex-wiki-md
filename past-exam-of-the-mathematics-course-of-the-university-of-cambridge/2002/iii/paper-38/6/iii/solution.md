<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An [ancillary statistic](../../../../../../ancillary-statistic.md) has a [sampling distribution](../../../../../../sampling-distribution.md) independent of the unknown parameter. It describes a realized aspect of the sample configuration without supplying a marginal [likelihood](../../../../../../likelihood-function.md) for the parameter. Its observed value can nevertheless be crucial to the precision of inference from the rest of the data. In a transitive [transformation model](../../../../../../transformation-model.md), invariance gives a common distribution under every parameter value, so [maximal invariants](../../../../../../maximal-invariant.md) provide natural ancillaries, such as the standardized configuration in a [location-scale family](../../../../../../location-scale-family.md).

Conditional inference uses the [sampling distribution](../../../../../../sampling-distribution.md) of an estimator or [sufficient statistic](../../../../../../sufficient-statistic.md) conditional on the observed ancillary. With joint coordinates $(T,A)$, the factorization

$$
f_\theta(t,a)=f_\theta(t\mid a)f_A(a)
$$

shows that the conditional [likelihood](../../../../../../likelihood-function.md) and the joint [likelihood](../../../../../../likelihood-function.md) differ only by a parameter-free data factor. Conditional reference distributions, [confidence intervals](../../../../../../confidence-interval.md) and [p-values](../../../../../../p-value.md) can still differ markedly from unconditional ones, because they adapt to the realized configuration. For a continuous ancillary one uses a [regular conditional distribution](../../../../../../regular-conditional-distribution.md) or [conditional density](../../../../../../conditional-density.md); dividing by the zero probability of a single ancillary value is not a valid definition.

An exact example makes this adaptation visible. Let independent observations be uniform on $(\theta-1/2,\theta+1/2)$, with $n\ge2$. Put $U=X_{(1)}$, $V=X_{(n)}$, $R=V-U$ and $C=(U+V)/2$. Specifying the minimum and maximum contributes $n(n-1)$ choices of observations, while each remaining observation must lie between them. Hence

$$
f_{U,V}(u,v)=n(n-1)(v-u)^{n-2},\quad \theta-\tfrac12<u<v<\theta+\tfrac12.
$$

The transformation $u=c-r/2$, $v=c+r/2$ has unit absolute [Jacobian determinant](../../../../../../jacobian-determinant.md). Its support is $0<r<1$, $|c-\theta|<(1-r)/2$. Integrating over $c$ gives

$$
f_R(r)=n(n-1)r^{n-2}(1-r),\qquad 0<r<1,
$$

which is independent of $\theta$, proving that the range is ancillary. Dividing the joint [density](../../../../../../density.md) by this marginal [density](../../../../../../density.md) gives

$$
C\mid R=r\sim\operatorname{Uniform}\left(\theta-\frac{1-r}2,\theta+\frac{1-r}2\right).
$$

The centered conditional pivot is uniform, so

$$
\boxed{\left[C-\frac{(1-\alpha)(1-R)}2,\ C+\frac{(1-\alpha)(1-R)}2\right]}
$$

has conditional coverage $1-\alpha$ at every $0<r<1$, and hence unconditional coverage $1-\alpha$ as well. A large realized range leaves little room for translating the interval and gives more precise inference. This is [range-conditioned uniform location inference](../../../../../../range-conditioned-uniform-location-inference.md). The range and center are not independent: the conditional spread depends on the range, even though the range is ancillary.

Completeness can give [independence](../../../../../../independent-random-variables.md) in other models. Suppose $S$ is a [complete sufficient statistic](../../../../../../complete-sufficient-statistic.md) and $A$ is ancillary. For any bounded [measurable](../../../../../../measurability.md) $h$, sufficiency makes $g(S)=E_\theta(h(A)\mid S)$ a function independent of $\theta$, while ancillarity makes $c=E_\theta h(A)$ independent of $\theta$. Since $E_\theta(g(S)-c)=0$ for every $\theta$, completeness implies $g(S)=c$ almost surely. Taking all bounded indicator functions $h$ proves [independence](../../../../../../independent-random-variables.md) of $A$ and $S$. This is the content of [Basu's theorem](../../../../../../basu-s-theorem.md), with the proof displaying precisely where sufficiency and completeness are used. Without completeness the conclusion fails: in the uniform location example the minimum and maximum are sufficient, and contain the nondegenerate ancillary range.

There are practical qualifications. Ancillaries need not be unique, and some models supply only approximate ancillary coordinates; one must specify the conditioning surface and the accuracy intended. Conditioning on a [statistic](../../../../../../statistic.md) sufficient for a [nuisance parameter](../../../../../../nuisance-parameter.md) is a different device: it may remove that nuisance even though the [statistic](../../../../../../statistic.md) is not ancillary for the full parameter. Conditioning indiscriminately can discard useful information. In higher-order [likelihood](../../../../../../likelihood-function.md) inference, the ancillary coordinates specify how the fitted data are varied, entering both the p\* [density](../../../../../../density.md) and the sample [derivatives](../../../../../../derivative.md) in the [modified profile likelihood](../../../../../../modified-profile-likelihood.md). Their role is therefore substantive, rather than merely a label for an extra [statistic](../../../../../../statistic.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
