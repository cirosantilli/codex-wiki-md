<h1 id="fagin-s-theorem">Fagin's theorem</h1>

↑ **Parent:** [Existential second-order logic](existential-second-order-logic.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fagin's_theorem)

Fix a finite relational [first-order signature](first-order-signature.md) $\tau$, and let $\mathcal K$ be a class of finite nonempty $\tau$-[first-order structures](first-order-structure.md) closed under [isomorphism](isomorphism.md). [Fagin's theorem](fagin-s-theorem.md) states that $\mathcal K$ is definable by one [existential second-order logic](existential-second-order-logic.md) sentence under [full semantics for second-order logic](full-semantics-for-second-order-logic.md) if and only if its language of standard finite encodings belongs to [NP](np-complexity.md). A standard encoding numbers the domain $\{0,\ldots,n-1\}$ and lists membership bits for each input relation, together with $n$; take an explicit encoding whose length is at least $n$. The encoding language contains all numbered copies of members of $\mathcal K$, with malformed encodings rejected. The [isomorphism](isomorphism.md) condition makes membership a property of the structure rather than an arbitrary choice of labels. Changing between the usual explicit encodings preserves the [NP](np-complexity.md) characterization by [polynomial time](polynomial-time.md) translations.

The forward direction is the witness-and-verifier calculation in [existential second-order logic](existential-second-order-logic.md). For the reverse direction, the guiding idea is to encode an accepting [nondeterministic computation](nondeterministic-turing-machine.md) using [second-order relation variables](second-order-relation-variable.md): fixed-length [tuples](finite-tuple.md) of domain elements index enough time steps and storage positions for a [polynomial time](polynomial-time.md) computation. A [first-order sentence](first-order-sentence.md) checks the initial input, legal transitions, and acceptance. The number of [tuples](finite-tuple.md) grows with the input, although the checking sentence stays fixed. No [total order](total-order.md) must be supplied as part of the input [first-order signature](first-order-signature.md): an auxiliary [total order](total-order.md) can itself be existentially guessed and constrained by a [first-order sentence](first-order-sentence.md). [Isomorphism](isomorphism.md) invariance ensures that a change of this auxiliary numbering does not change membership in $\mathcal K$.

The [second-order encoding of three-colorability](second-order-encoding-of-three-colorability.md) is a small instance of the forward direction. The beauty of [Fagin's theorem](fagin-s-theorem.md) is the complete correspondence: the computational class [NP](np-complexity.md) can be characterized by the shape of a logical description, without mentioning a particular machine in the statement. The scope is finite relational [first-order structures](first-order-structure.md) and fixed sentences; it is not a claim about deciding arbitrary [second-order logic](second-order-logic.md) sentences or about arbitrary infinite domains.

Ronald Fagin published the result in [Generalized First-Order Spectra and Polynomial-Time Recognizable Sets, SIAM-AMS Proceedings 7 (1974), pp. 43–73, Section 4](https://s3.us.cloud-object-storage.appdomain.cloud/res-files/500-genspec.pdf). The original paper frames the correspondence using classes of finite expansions and their encodings. Fagin's [author-maintained publication list](https://ronfagin.com/papers/) explains that the abstract in the available copy was added in 2019; its modern summary should therefore not be mistaken for part of the 1974 printing.

## ↑ Ancestors (7)

1. [Existential second-order logic](existential-second-order-logic.md)
2. [Second-order logic](second-order-logic.md)
3. [Mathematical logic](mathematical-logic-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Existential second-order logic](existential-second-order-logic.md)
- [Fagin's theorem](fagin-s-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-23/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-23/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-23/7/c/solution.md)
