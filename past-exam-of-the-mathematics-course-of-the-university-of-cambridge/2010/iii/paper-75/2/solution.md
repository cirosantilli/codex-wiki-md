<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Here [Cartesian category](../../../../../cartesian-category.md) means a category with all [finite limits](../../../../../finite-limit.md). Let $m:Y\hookrightarrow X$ be a [monomorphism](../../../../../monomorphism.md), and let $\varepsilon_X\hookrightarrow X\times PX$ be universal membership for a [power object](../../../../../power-object.md) $PX$. Pull it back to $Y\times PX$ and then regard the result as a [subobject](../../../../../subobject.md) of $X\times PX$. Its unique classifier is an endomorphism $r:PX\to PX$: on a parameterized subobject it intersects with $Y$. Intersecting twice has the same result as intersecting once, so uniqueness of classification gives $r^2=r$.

Take the [equalizer](../../../../../equaliser.md) $q:Q\hookrightarrow PX$ of $r$ and the identity, and restrict membership to $Y\times Q$. For any [subobject](../../../../../subobject.md) $S\hookrightarrow Y\times Z$, its composite with $m\times1_Z$ is a [subobject](../../../../../subobject.md) of $X\times Z$, hence is uniquely classified by $s:Z\to PX$. Since it is contained in $Y\times Z$, its intersection with that subobject changes nothing, so $rs=s$ and $s$ factors uniquely through $Q$. Conversely every map $Z\to Q$ gives the original kind of family by pulling back the restricted membership. These inverse operations give

$$
\boxed{\mathcal C(Z,Q)\cong\operatorname{Sub}(Y\times Z)},
$$

naturally in $Z$. Thus $Q$ is a [power object of a subobject](../../../../../power-object-of-a-subobject.md), even if no power objects other than $PX$ were assumed.

Now consider the [slice category](../../../../../slice-category.md) $\mathcal E/A$, which has [finite limits](../../../../../finite-limit.md) formed by ambient pullbacks and has terminal object $1_A:A\to A$. The constant family $A\times X\to A$ has slice [power object](../../../../../power-object.md) $A\times PX\to A$: for $Z\to A$,

$$
(A\times X)\times_A Z\cong X\times Z,
$$

and a classifier $Z\to PX$ is equivalently the map $Z\to A\times PX$ over $A$. Every family $p:X\to A$ is a [subobject](../../../../../subobject.md) of this constant family through its monic graph $(p,1_X):X\hookrightarrow A\times X$. Apply the first construction inside the slice. **Consequently every slice of a Cartesian category with power objects again has power objects.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
