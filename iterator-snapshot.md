# Iterator snapshot

↑ **Parent:** [Iterator](iterator.md)

A new cursor with the same remaining [sequence](sequence.md) and an independent consumption position. Copying only a wrapper that still points to the same destructive source does not suffice: that gives [shared iterator consumption](shared-iterator-consumption.md). Cached lookahead and phase flags are part of the state that a snapshot must preserve. Element values need not be deep-copied merely to duplicate the cursor.

**Table of contents**

- [Memoized iterator snapshot](memoized-iterator-snapshot.md)
  - [Memoized successor chain for stateful iterator copies](memoized-successor-chain-for-stateful-iterator-copies.md)

## ↑ Ancestors (4)

1. [Iterator](iterator.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/object-oriented-programming/2/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/object-oriented-programming/2/f/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming-resit/7/a/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/6/a/solution.md)
- [Prefix-dropping iterator](prefix-dropping-iterator.md)
