# Debounced toggle switch

↑ **Parent:** [Finite-state machine](finite-state-machine.md)

A sampled toggle controller can reject short disturbances by requiring three consecutive high samples to toggle, and then three consecutive low samples before another high run is allowed to toggle. One four-[bit](bit.md) [synchronous sequential circuit](synchronous-sequential-circuit.md) stores output $z$, an armed [bit](bit.md) $e$, and input history $p,q$. Initially $(p,q,e,z)=(0,0,1,0)$. Set

$$
c=a\land p\land q,\qquad d=\neg a\land\neg p\land\neg q,
\qquad(p',q')=(a,p),\qquad e'=d\lor(e\land\neg c),\qquad
z'=z\oplus(e\land c).
$$

The two [three-sample run detectors](three-sample-run-detector.md) cannot assert simultaneously. A high run toggles once and clears $e$; only a complete low run rearms it. All right-hand sides use the old state, so the toggling event occurs at the third qualifying [clock edge](clock-edge.md).

The controller has twelve distinguishable behaviours: for each $z$, three armed states count trailing highs of lengths $0,1,2$, and three disarmed states count trailing lows of lengths $0,1,2$. The run lengths are distinguished by the number of further matching samples needed before a toggle or rearm. Armed and disarmed states are distinguished by an all-high continuation. Thus at least $\lceil\log_2 12\rceil=4$ state [bits](bit.md) are required, and the displayed design attains that bound.

## ↑ Ancestors (6)

1. [Finite-state machine](finite-state-machine.md)
2. [Formal language theory](formal-language-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/3/c/solution.md)
