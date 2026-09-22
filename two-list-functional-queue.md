# Two-list functional queue

↑ **Parent:** [FIFO queue](fifo-queue.md)

Represent the abstract sequence by `front @ rev rear`. Keep the front nonempty unless both lists are empty. Prepending to the rear enqueues; when the front is exhausted, reverse the rear once. Along a single sequence of uses, each element crosses between lists at most once, giving constant [amortized analysis](amortized-analysis.md) cost per operation. Reusing an old persistent version can repeat a reversal and needs a separate analysis.

// Destination: computer-science.bigb

## ↑ Ancestors (4)

1. [FIFO queue](fifo-queue.md)
2. [Data structure](data-structure.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/5/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-5/5/a/iii/solution.md)
