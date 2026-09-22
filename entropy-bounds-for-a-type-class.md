# Entropy bounds for a type class

↑ **Parent:** [Method of types](method-of-types.md)

For an attainable [empirical distribution](type-information-theory.md) $q$ on a fixed finite [alphabet](alphabet.md) of size $m$,

$$
(n+1)^{-m}e^{nH_e(q)}\leq |T_n(q)|\leq e^{nH_e(q)}.
$$

Thus $\ln|T_n(q)|$ differs from $nH_e(q)$ by at most $m\ln(n+1)$, uniformly over attainable profiles. [Information entropy](information-entropy-split.md) is the leading logarithmic count; the polynomial factor matters at short lengths.[§II, Lemma II.2, equation (II.4), printed pp. 2506–2507: type-class cardinality bounds](the-method-of-types-by-imre-csiszar.md)

The upper bound has a short explanation. Under an [independent and identically distributed](independent-and-identically-distributed-random-variables.md) source whose law is $q$ itself, each string in $T_n(q)$ has [probability](probability.md) $e^{-nH_e(q)}$. Multiplying by the number of such strings cannot give a [probability](probability.md) above one. A corresponding polynomial lower bound follows from the [multinomial coefficient](multinomial-coefficient.md); the [Stirling's approximation](stirling-formula.md) gives sharper prefactors when needed.

For the balanced four-symbol class, $H_e(q)=\ln2$, so the upper bound is $e^{4\ln2}=16$, while the exact size is six. [Information entropy](information-entropy-split.md) is not an exact count for a short string. On the leading scale it becomes precise: the difference divided by $n$ tends to zero as $n$ grows with the [alphabet](alphabet.md) fixed.

## ↑ Ancestors (7)

1. [Method of types](method-of-types.md)
2. [Type (information theory)](type-information-theory.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Probability of a type class](probability-of-a-type-class.md)
