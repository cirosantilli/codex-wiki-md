# Stage histories appear below every limit constructible level

↑ **Parent:** [Coded relative constructible stage](coded-relative-constructible-stage.md)

For a [transitive set](transitive-set.md) $X$, let $f_\xi$ be the history function $\eta\mapsto L_\eta(X)$ on $\xi+1$ in the [relative constructible hierarchy](relative-constructible-hierarchy.md). By [transfinite induction](transfinite-induction.md), $f_\xi\in L_{\xi+k}(X)$ for some finite $k$, possibly depending on $\xi$. The base and successor steps follow by forming finite [ordered pairs](ordered-pair.md) and adjoining the next entry, using $L_{\xi+1}(X)\in L_{\xi+2}(X)$. These operations require finitely many subsequent [definable power sets](definable-power-set-split.md).

At a nonzero [limit ordinal](limit-ordinal.md) $\lambda$, the inductive bounds put every earlier $f_\eta$ in $L_\lambda(X)$, since $\eta+k<\lambda$. This level satisfies [finite relation closure for set-theoretic coding](finite-relation-closure-for-set-theoretic-coding.md), independently of the availability of history functions. Consequently its [coded relative constructible stage](coded-relative-constructible-stage.md) predicate computes the endpoints correctly. Finite pairing closure and the earlier histories show that

$$
h=\{\langle\eta,B\rangle\in L_\lambda(X):(L_\lambda(X),\in)\models S_X(\eta,B)\}
$$

contains exactly the pairs $\langle\eta,L_\eta(X)\rangle$ for $\eta<\lambda$. There are no extra indices: if $\eta\geq\lambda$ and $B=L_\eta(X)\in L_\lambda(X)$, increasing levels would give $B\in B$, contradicting [Axiom of foundation](axiom-of-regularity.md). Thus $h=f_\lambda\!\upharpoonright\lambda$ is a definable [subset](subset.md) of $L_\lambda(X)$ and belongs to $L_{\lambda+1}(X)$. Extracting its domain $\lambda$ and adjoining $\langle\lambda,L_\lambda(X)\rangle$ uses finitely many further operations, proving the induction step. Every nonzero limit $\alpha$ therefore contains all $f_\xi$ with $\xi<\alpha$, as required by [relative constructible level recognition](relative-constructible-level-recognition.md).

## ↑ Ancestors (11)

1. [Coded relative constructible stage](coded-relative-constructible-stage.md)
2. [Relative constructible hierarchy](relative-constructible-hierarchy.md)
3. [Relative constructible universe](relative-constructible-universe.md)
4. [Constructible universe](constructible-universe.md)
5. [Constructible hierarchy](constructible-hierarchy.md)
6. [Definable power set](definable-power-set-split.md)
7. [Set theory](set-theory-split.md)
8. [Foundations of mathematics](foundations-of-mathematics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Coded relative constructible stage](coded-relative-constructible-stage.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-121/2/iii/solution.md)
