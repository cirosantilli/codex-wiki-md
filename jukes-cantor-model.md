# Jukes-Cantor model

↑ **Parent:** [Nucleotide substitution](nucleotide-substitution.md)

The [Jukes-Cantor model](jukes-cantor-model.md) is a symmetric four-state [continuous-time Markov chain](continuous-time-markov-chain-split.md) for [DNA](deoxyribonucleic-acid.md) evolution. Each change to a specified different base has rate $q$, so the total rate of actual changes is $3q$. Its same-base probability is $1/4+(3/4)e^{-4qt}$ and its probability for one specified different base is $(1/4)(1-e^{-4qt})$. The probability of any mismatch is three times the latter, tending to $3/4$ at long times. Distinguish the exponent parameter $4q$ from the actual per-site [mutation rate](mutation-rate.md) $3q$ when fitting this model.

## ↑ Ancestors (6)

1. [Nucleotide substitution](nucleotide-substitution.md)
2. [Point mutation](point-mutation.md)
3. [Mutation](mutation.md)
4. [Genetics](genetics-split.md)
5. [Biology](biology-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Jukes-Cantor model](jukes-cantor-model.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2024/paper-2/c9/a/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/3/b/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/3/c/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-2/3/d/solution.md)
