# Almost strongly universal hash family

↑ **Parent:** [Hash function](hash-function.md)

An [almost strongly universal hash family](almost-strongly-universal-hash-family.md) relaxes the exact [ordered pair](ordered-pair.md) balance of a [strongly universal hash family](strongly-universal-hash-family.md). In the convention used here, choose $h$ with the [uniform distribution on a finite set](discrete-uniform-distribution.md) from a family with $q$ possible [outputs](output-computing.md). Every individual [output](output-computing.md) remains uniform, and for every distinct pair of [inputs](input-computer-science.md) $x,y$ and every specified [ordered pair](ordered-pair.md) of [outputs](output-computing.md) $u,v$,

$$
\Pr_h[h(x)=u,h(y)=v]\leq\frac{\varepsilon}{q}.
$$

Equivalently, the [conditional probability](conditional-probability.md) $\Pr_h[h(y)=v\mid h(x)=u]$ is at most $\varepsilon$. This asks how predictable a second [output](output-computing.md) can become after the first is known.

For $q=5$, [strongly universal hash families](strongly-universal-hash-family.md) give $\varepsilon=1/5$: learning one [output](output-computing.md) leaves each specified second [output](output-computing.md) with [conditional probability](conditional-probability.md) $1/5$. A looser guarantee $\varepsilon=2/5$ permits a specified [ordered pair](ordered-pair.md) to have [probability](probability.md) as large as $2/25$, while each individual [output](output-computing.md) still has [probability](probability.md) $1/5$. Summing over the five equal [ordered pairs](ordered-pair.md) bounds the collision [probability](probability.md) by $2/5$, rather than the $1/5$ required of a [universal hash family](universal-hash-family.md). Thus an [almost strongly universal hash family](almost-strongly-universal-hash-family.md) need not be a [universal hash family](universal-hash-family.md). Necessarily $\varepsilon\geq1/q$, because the $q$ conditional [probabilities](probability.md) sum to one; equality recovers a [strongly universal hash family](strongly-universal-hash-family.md). This relaxation is useful in [Wegman–Carter authentication](wegman-carter-authentication.md), where efficiency can be traded against a quantified forgery bound within a complete [message authentication](message-authentication.md) protocol.

**Table of contents**

- [Polynomial almost strongly universal hashing](polynomial-almost-strongly-universal-hashing.md)

## ↑ Ancestors (3)

1. [Hash function](hash-function.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Almost strongly universal hash family](almost-strongly-universal-hash-family.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-54/3/solution.md)
- [Wegman–Carter authentication](wegman-carter-authentication.md)
