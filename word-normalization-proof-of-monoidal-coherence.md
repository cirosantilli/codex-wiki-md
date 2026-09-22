# Word normalization proof of monoidal coherence

↑ **Parent:** [Monoidal coherence theorem](monoidal-coherence-theorem.md)

Associate to a finite ordered word $w$ the right-associated tensor $N(w)$, retaining a terminal unit: $N(\varnothing)=I$ and $N(Aw)=A\otimes N(w)$. Define concatenation maps recursively by

$$
c_{\varnothing,v}=\lambda_{N(v)},\qquad
c_{Au,v}=(1_A\otimes c_{u,v})a_{A,N(u),N(v)}.
$$

The [unit identities derived from the monoidal pentagon and triangle](unit-identities-derived-from-the-monoidal-pentagon-and-triangle.md) give $c_{u,\varnothing}=\rho_{N(u)}$. Induction on $u$, using the pentagon in the induction step and left-unitor compatibility in the base case, gives

$$
c_{uv,w}(c_{u,v}\otimes1)=c_{u,vw}(1\otimes c_{v,w})a_{N(u),N(v),N(w)}.
$$

Normalize a letter by $\rho_A^{-1}$, a formal unit by $1_I$, and a tensor expression recursively using $c$. The displayed identities show that normalization commutes with each generating [associator](associator.md) or [unitor](unitor.md), and therefore also with inverses, tensor products and composites of them. Every structural arrow from expression $S$ to expression $T$ is consequently $\nu_T^{-1}\nu_S$, proving [monoidal coherence](monoidal-coherence-theorem.md) without presupposing it.

## ↑ Ancestors (7)

1. [Monoidal coherence theorem](monoidal-coherence-theorem.md)
2. [Monoidal category](monoidal-category.md)
3. [Category theory](category-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-25/6/solution.md)
