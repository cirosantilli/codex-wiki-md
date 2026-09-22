<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

We prove both versions. In the [general adjoint functor theorem](../../../../../freyd-general-adjoint-functor-theorem.md), let $G:\mathcal D\to\mathcal C$ be a [functor](../../../../../functor.md) between locally small categories, with $\mathcal D$ complete. Then $G$ has a left adjoint if and only if it preserves small limits and satisfies the [solution-set condition](../../../../../solution-set-condition.md): for each $C\in\mathcal C$ there is a set of arrows $u_i:C\to GD_i$ such that every arrow $u:C\to GD$ factors as $G(h)u_i$ for some $i$ and $h:D_i\to D$.

First prove the [initial-object lemma for complete categories with a weakly initial set](../../../../../initial-object-lemma-for-complete-categories-with-a-weakly-initial-set.md). Let $\mathcal A$ be locally small and complete, and have a small weakly initial family $(W_i)$. Its product $W$ is weakly initial: a map $W_i\to A$ can be composed with the product projection. Take $e:E\to W$ to be the simultaneous [equalizer](../../../../../equaliser.md) of every endomorphism of $W$ and its identity. This is a small limit since $\mathcal A(W,W)$ is a set. Maps $E\to A$ exist by composing $e$ with a weakly initial map $W\to A$.

For uniqueness, take any $a,b:E\to A$ and their [equalizer](../../../../../equaliser.md) $j:Z\to E$. Weak initiality of $W$ gives $t:W\to Z$. The endomorphism $ejt$ of $W$ fixes $e$ by its defining [equalizer](../../../../../equaliser.md) property, so $ejte=e$. Since $e$ is monic, $jte=1_E$. Thus $j$ is both monic and split epic, hence invertible, forcing $a=b$. Therefore $E$ is initial. This proves the lemma without an unproved initial-object assertion.

Now fix $C\in\mathcal C$. The comma category $(C\downarrow G)$ is locally small. It is complete: take the limit of the underlying diagram in $\mathcal D$, use preservation by $G$ to factor the compatible arrows from $C$, and obtain the universal comma cone. The solution set is exactly a small weakly initial family in this comma category. The lemma provides its [initial object](../../../../../initial-object.md) $(FC,\eta_C)$. Its universal property is the natural bijection $\mathcal D(FC,D)\cong\mathcal C(C,GD)$. For $v:C\to C'$, initiality gives the unique $Fv$ satisfying $G(Fv)\eta_C=\eta_{C'}v$; uniqueness proves identities and composition. Thus these objects form a left adjoint. Conversely a left adjoint provides the singleton solution set consisting of its unit arrow, and a right adjoint preserves limits: the [adjunction](../../../../../adjoint-functors.md) bijections identify cones into the image diagram with cones from the corresponding left-adjoint object into the original diagram. This proves both directions of the general theorem.

The [limit form of the special adjoint functor theorem](../../../../../limit-form-of-the-special-adjoint-functor-theorem.md) assumes instead that $\mathcal D$ is complete, locally small and well-powered, and has a small cogenerating family $(Q_i)$. For any locally small target, a [functor](../../../../../functor.md) $G:\mathcal D\to\mathcal C$ has a left adjoint exactly when it preserves small limits. Necessity is already proved. For sufficiency we construct a solution set, so that the general theorem applies.

Fix $C$. Given $u:C\to GD$, consider all pairs $h,k:D\to Q_i$ with $G(h)u=G(k)u$. There is only a set of these pairs. Intersect their [equalizers](../../../../../equaliser.md) to obtain a [monomorphism](../../../../../monomorphism.md) $m:D'\to D$. Since $G$ preserves this limit and $u$ equalizes the images of all pairs, it factors uniquely as $u=G(m)u'$ for $u':C\to GD'$.

For each realized pair $(i,v)$ with $v=G(h)u:C\to GQ_i$, choose one such $h$. Any other $k$ with the same pair restricts to the same map on $D'$. The restricted chosen maps jointly separate morphisms into $D'$: if two such morphisms become equal after all chosen maps, they become equal after every $hm$, and the cogenerating family then makes their composites with $m$ equal; monicity of $m$ cancels it. Hence the resulting map

$$
D'\longrightarrow\prod_{(i,v)\in J}Q_i
$$

is monic, where $J$ is a subset of the fixed set $\coprod_i\mathcal C(C,GQ_i)$.

There is only a set of possible $J$, a set of subobjects of each corresponding product by well-poweredness, and a set of arrows from $C$ into $G$ of each chosen subobject representative by local smallness of $\mathcal C$. Collect all these representative comma objects. The factorization just constructed shows that they form a weakly initial set in $(C\downarrow G)$. This is the [cogenerator bound for comma-category solution sets](../../../../../cogenerator-bound-for-comma-category-solution-sets.md), with realized subsets avoiding any assumption that all proposed maps to cogenerators have lifts. The general theorem now gives the left adjoint and proves the special theorem.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
