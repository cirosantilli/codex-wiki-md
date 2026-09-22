# Trace learning

↑ **Parent:** [Hebbian learning](hebbian-learning.md)

A local association rule uses a decaying activity trace to connect representations encountered at nearby times. One implementation has $\bar y_i(t)=\rho\bar y_i(t-1)+(1-\rho)y_i(t)$ and $\Delta w_{ij}=\eta\bar y_i(t-1)x_j(t)$, followed by [synaptic normalization](synaptic-normalization.md). Temporal continuity can link distinct views of one object, but a trace spanning an identity change can create a false association.[Abstract; Neural Computation 3, pp. 194–200, transformation-sequence learning](learning-invariance-from-transformation-sequences-by-peter-foldiak.md)

## ↑ Ancestors (9)

1. [Hebbian learning](hebbian-learning.md)
2. [Unsupervised learning](unsupervised-learning.md)
3. [Statistical learning](statistical-learning-split.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Eligibility trace](eligibility-trace.md)
- [Invariant object recognition with trace learning and multiple stimuli present during training by Simon M. Stringer and others](invariant-object-recognition-with-trace-learning-and-multiple-stimuli-present-during-training-by-simon-m-stringer-and-others.md)
- [Solution](past-exam-of-the-computational-neuroscience-course-of-the-university-of-oxford/2022/4/solution.md)
- [Solution](past-exam-of-the-episodic-and-semantic-memory-course-of-the-university-of-oxford/2022/5/solution.md)
- [Statistical separation of objects in clutter](statistical-separation-of-objects-in-clutter.md)
- [Symmetric coactivity weights do not distinguish reversed episodes](symmetric-coactivity-weights-do-not-distinguish-reversed-episodes.md)
