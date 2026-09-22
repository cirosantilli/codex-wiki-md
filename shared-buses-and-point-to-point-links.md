# Shared buses and point-to-point links

↑ **Parent:** [Computer bus](computer-bus.md)

The word “bus” is also used for interconnect families that do not give all components a single shared electrical path. Intel's [An Introduction to the Intel QuickPath Interconnect](https://www.intel.com/content/dam/doc/white-paper/quick-path-interconnect-introduction-paper.pdf) (January 2009, p. 8, “Interconnect Overview”) explicitly describes [Intel QuickPath Interconnect](intel-quickpath-interconnect.md) as a point-to-point link despite the serial-bus terminology, and compares it with [PCI Express](pci-express.md). Here each link connects two endpoints. Independent links can carry traffic concurrently; traffic converging on one link or target still competes for that resource. The [shared-bus timing example](shared-bus-timing-example.md)'s single owner and serialized service must therefore not be assumed for a whole network of links merely because its interfaces are called buses. Serial versus parallel transfer and shared versus point-to-point topology are separate distinctions.

## ↑ Ancestors (3)

1. [Computer bus](computer-bus.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Intel QuickPath Interconnect](intel-quickpath-interconnect.md)
- [PCI Express](pci-express.md)
