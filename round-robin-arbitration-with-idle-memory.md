# Round-robin arbitration with idle memory

↑ **Parent:** [Round-robin arbitration](round-robin-arbitration.md)

Store both the last recipient index $L$ and a current-grant valid [bit](bit.md) $V$. With $k$ possible recipients, an idle period clears $V$ while preserving $L$. The [Moore machine](moore-machine.md) grants requester $j$ precisely when $V\land[L=j]$ holds. For $k>1$, its $k$ idle states are distinguishable by a subsequent pair of competing requests with different positions in the cyclic order; active states have distinct outputs. Thus all $2k$ states are distinguishable and $\lceil\log_2(2k)\rceil$ state bits suffice and are necessary for this output convention. A continuously asserted request receives a grant within $k$ decisions, because before that grant the cyclic scan cannot pass it to choose a later asserted request.

## ↑ Ancestors (4)

1. [Round-robin arbitration](round-robin-arbitration.md)
2. [Digital electronics](digital-electronics.md)
3. [Electrical engineering](electrical-engineering-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/digital-systems-linear-algebra-introduction-to-formal-proof/1/b/solution.md)
