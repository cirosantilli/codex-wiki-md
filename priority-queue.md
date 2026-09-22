# Priority queue

↑ **Parent:** [Data structure](data-structure.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Priority_queue)

A [priority queue](priority-queue.md) stores items with comparable priority keys and supports insertion, inspection of a best-priority item, and removal of a best-priority item. Here we use the minimum convention: keys have a [total order](total-order.md), and smaller means earlier. The operation `peek` returns a stored item of [minimum](minimum-of-a-subset-of-a-total-order.md) priority without removing it; `extract-min` removes and returns such an item. Both require a nonempty [priority queue](priority-queue.md), or an explicitly specified empty-case result. A maximum-oriented [priority queue](priority-queue.md) reverses the choice.

For the requests $(5,\mathrm{Ada}),(2,\mathrm{Bo}),(4,\mathrm{Cy})$, `peek` returns Bo and leaves all three requests stored. `extract-min` returns Bo and leaves Ada and Cy; another `peek` returns Cy. Inserting $(1,\mathrm{Dee})$ now makes Dee the next request selected. This changing collection need not be a [sorted array](sorted-array.md): only the next choice must be available.

Distinct items may share a priority. Inserting $(2,\mathrm{Eli})$ alongside $(2,\mathrm{Bo})$ permits either item to be removed first. A [priority queue](priority-queue.md) does not inherently promise arrival order on ties. If that policy matters, compare priority first and a unique increasing arrival number second; the resulting [total order](total-order.md) makes earlier arrivals win equal-priority ties. This is analogous to the motivation for [stable sorting](stable-sorting.md), but it is an extra policy for the [priority queue](priority-queue.md).

The interface specifies behavior; the [data structure](data-structure.md) determines costs. A [binary heap](binary-heap.md) implements a [priority queue](priority-queue.md) with constant-time `peek` and logarithmic-time insertion and `extract-min`, under the cost assumptions below. Scheduling by urgency or by the time of the next event needs exactly this repeated next-item selection. MIT's notes use these applications to motivate the [priority queue](priority-queue.md) interface.[MIT 6.006, lecture 8: priority queues and binary heaps, pp. 1–2](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/40d4851e550507ca14dc778b9b2266cc_MIT6_006S20_lec8.pdf)

**Table of contents**

- [Binary heap](binary-heap.md)
  - [Heap order](heap-order.md)
  - [Sift up](sift-up.md)
  - [Sift down](sift-down.md)

## ↑ Ancestors (3)

1. [Data structure](data-structure.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Binary heap](binary-heap.md)
- [Data structure](data-structure.md)
- [Dijkstra algorithm](dijkstra-algorithm.md)
- [Priority queue](priority-queue.md)
- [Ready queue](ready-queue.md)
