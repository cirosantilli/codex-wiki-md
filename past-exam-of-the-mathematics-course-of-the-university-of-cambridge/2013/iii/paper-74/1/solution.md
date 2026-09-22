<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take the definition of an [elementary topos](../../../../../elementary-topos.md) as a category with [finite limits](../../../../../finite-limit.md), [exponential objects](../../../../../exponential-object.md) and a [subobject classifier](../../../../../subobject-classifier.md) $\top:1\hookrightarrow\Omega$. Its [power object](../../../../../power-object.md) is $PX=\Omega^X$, and $Pf:PY\to PX$ is precomposition with $f:X\to Y$. Transposing a predicate on $X\times Y$ in either variable gives

$$
\mathcal E(X,PY)\cong\mathcal E(Y,PX).
$$

Thus $P^{\mathrm{op}}:\mathcal E\to\mathcal E^{\mathrm{op}}$ is left adjoint to the [contravariant power-object functor](../../../../../contravariant-power-object-functor.md) $P:\mathcal E^{\mathrm{op}}\to\mathcal E$.

Here are the remaining hypotheses for the [crude monadicity theorem](../../../../../crude-monadicity-theorem.md), obtained from those [topos](../../../../../elementary-topos.md) axioms. The unit of this [adjunction](../../../../../adjoint-functors.md) is $\eta_X:X\to PPX$, internally $\eta_X(x)(S)=(x\in S)$. It is monic: if two such evaluations agree, evaluate on the singleton predicate $\{x\}$ classified by the diagonal to obtain $x=y$. If $Pf$ is invertible, naturality $PPf\,\eta_X=\eta_Yf$ therefore makes $f$ monic. The characteristic map of this mono, regarded as a global element of $PY$, pulls back along $f$ to the everywhere-true predicate on $X$. Since $Pf$ is monic, that characteristic map was already everywhere true on $Y$. The classifier [pullback](../../../../../pullback-category-theory.md) then says that $f$ is invertible. Hence $P$ is a [conservative functor](../../../../../conservative-functor.md).

It remains to check preservation of [reflexive coequalizers](../../../../../reflexive-coequalizer.md) in the opposite category. Equivalently, let $f,g:B\rightrightarrows A$ be a [coreflexive pair](../../../../../coreflexive-pair.md), with $r:A\to B$ satisfying $rf=rg=1_B$, and let $e:E\hookrightarrow B$ be their [equalizer](../../../../../equaliser.md). Both $f$ and $g$ are monic. For any mono $i$, there is a direct-image map $\exists_i$ between [power objects](../../../../../power-object.md): a [subobject](../../../../../subobject.md) is sent to its composite with $i$. This uses only classification of monos, not the prior existence of general images or colimits. We have $Pi\,\exists_i=1$.

For a predicate $W\hookrightarrow B$, consider its direct image along $f$. Its [pullbacks](../../../../../pullback-category-theory.md) along the two sections are

$$
Pf\,\exists_f(W)=W,\qquad
Pg\,\exists_f(W)=W\cap E=\exists_e Pe(W).
$$

To verify the second equality, $g(b)=f(w)$ with $w\in W$ implies $b=w$ after applying $r$, and therefore $f(b)=g(b)$; conversely $b\in W\cap E$ supplies that witness. This argument works for parameterized [subobjects](../../../../../subobject.md) as well, so it is an equality of arrows between [power objects](../../../../../power-object.md).

Now if $h:PB\to Z$ satisfies $hPf=hPg$, then $h=h\exists_e Pe$. Hence $h\exists_e:PE\to Z$ is its unique factorization through $Pe$, uniqueness following from the section $\exists_e$. Therefore

$$
PA\mathrel{\substack{\xrightarrow{Pf}\\[-2pt]\xrightarrow[\ ]{Pg}}}PB\xrightarrow{Pe}PE
$$

is a [coequalizer](../../../../../coequalizer.md). [Finite limits](../../../../../finite-limit.md) supply every required coreflexive [equalizer](../../../../../equaliser.md). The right adjoint $P$ reflects isomorphisms and preserves the corresponding reflexive [coequalizers](../../../../../coequalizer.md), so **$P$ is monadic**. In particular $\mathcal E^{\mathrm{op}}$ is equivalent to the [Eilenberg-Moore category](../../../../../eilenberg-moore-category.md) of the double-power-object monad on $\mathcal E$.

Let $F:\mathcal E\to\mathcal F$ be a [logical functor](../../../../../logical-functor.md), and suppose $L\dashv F$. Preservation of exponentials and the classifier gives $F P_{\mathcal E}\cong P_{\mathcal F}F^{\mathrm{op}}$, compatibly with the units, counits and resulting monads. Thus $F^{\mathrm{op}}$ is the algebra [functor](../../../../../functor.md) lifting the base [functor](../../../../../functor.md) $F$ through the two monadic power-object [functors](../../../../../functor.md). The [adjoint lifting theorem for monad algebra functors](../../../../../adjoint-lifting-theorem-for-monad-algebra-functors.md) applies to the base [adjunction](../../../../../adjoint-functors.md) $L\dashv F$: its required [coequalizers](../../../../../coequalizer.md) exist in $\mathcal E^{\mathrm{op}}$, because $\mathcal E$ has finite [equalizers](../../../../../equaliser.md). It supplies a left adjoint $K\dashv F^{\mathrm{op}}$. Taking opposites gives **$F\dashv K^{\mathrm{op}}$**, the required right adjoint to $F$.

Preserving either of the two logical structures by itself is insufficient. For the exponential example take **$F:\mathbf{Set}\to\mathbf{Set}$ constant at $1$**. The constant-empty [functor](../../../../../functor.md) is its left adjoint, since both relevant hom-sets are singletons. Its canonical exponential comparison is $1\cong1^1$, so it preserves exponentials. It has no right adjoint: a [functor](../../../../../functor.md) with a right adjoint would preserve the initial object, whereas $F(\varnothing)=1$.

For the classifier example take **$G:(\mathbb Z/2)\text{-}\mathbf{Set}\to\mathbf{Set}$ to be fixed points**. The trivial-action [functor](../../../../../functor.md) is left adjoint to $G$. In a group-action [topos](../../../../../elementary-topos.md) the classifier is the trivial-action two-element set, since invariant subsets have ordinary equivariant characteristic maps. Therefore $G$ preserves the classifier, its true arrow and the terminal object. But $G$ does not preserve the [coequalizer](../../../../../coequalizer.md) of the identity and the nontrivial translation on the regular two-element group set: that [coequalizer](../../../../../coequalizer.md) is $1$, while the fixed-point sets of the domain and codomain of the parallel pair are empty. Their set-theoretic [coequalizer](../../../../../coequalizer.md) is empty, not $G(1)=1$. Thus $G$ has no right adjoint.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
