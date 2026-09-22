# Information projection and rare sample means

↑ **Parent:** [Relative entropy minimization under a mean constraint](relative-entropy-minimization-under-a-mean-constraint.md)

Take [independent and identically distributed](independent-and-identically-distributed-random-variables.md) draws from the uniform three-outcome reference above. An observed sample [mean](expected-value.md) at least $1/2$ is unusual because the source [expected value](expected-value.md) is zero. For two draws, the only successful ordered pairs are $(0,1),(1,0),(1,1)$, giving [probability](probability.md) $3/9=1/3$.

For long samples, the relevant [empirical distributions](type-information-theory.md) have [mean](expected-value.md) at least $1/2$. The [method of types](method-of-types.md) assigns a profile $q$ a leading probability cost $e^{-nD(q\Vert p)}$. The least costly admissible profile is the [information projection on three outcomes](information-projection-on-three-outcomes.md): in this example the minimizing [mean](expected-value.md) is on the boundary $1/2$, and the leading exponent is approximately $0.197378$ [nats](nat-unit.md) per draw. The exponential scale is not an exact finite-sample probability formula.[§12.1, Theorem 12.1, equation (12.2), printed p. 131; §12.2, Theorem 12.3, printed p. 134](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-12-information-projection-and-large-deviation.md)

The attraction of this connection is that a constrained optimization problem predicts the most probable way an unusual aggregate observation can occur. It links [relative entropy](kullback-leibler-divergence.md), [expected value](expected-value.md) constraints and rare [empirical distributions](type-information-theory.md) without identifying a rare event with just one exact attainable [type class](type-class.md).

## ↑ Ancestors (9)

1. [Relative entropy minimization under a mean constraint](relative-entropy-minimization-under-a-mean-constraint.md)
2. [Information projection](information-projection.md)
3. [Method of types](method-of-types.md)
4. [Type (information theory)](type-information-theory.md)
5. [Information theory](information-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
