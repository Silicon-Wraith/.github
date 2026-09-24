<p align="center">
  <img src="../assets/Silicon_Wraith-Logo.png"
       alt="Silicon Wraith"
       width="700">
</p>

<h3 align="center">
  Software that lives between the machines.
</h3>

Silicon Wraith is an open-source software organization focused on distributed
systems, autonomous software, AI-assisted engineering, and the infrastructure
that connects them.

The name reflects a recurring theme in the projects here: software that isn't
defined by a single machine or process, but operates across systems — coordinating,
communicating, adapting, and doing useful work largely out of sight.

## Projects

### Nebulon

### Nebulon

**A censorship-resistant, self-organizing peer-to-peer network built around
per-connection polymorphic protocols.**

#### The problem

Decentralized networks often become identifiable and controllable through the
very mechanisms that allow them to function. Protocol signatures can be
fingerprinted. Bootstrap infrastructure can become a target. Distributed hash
tables and discovery mechanisms expose recognizable behavior. Even when the
content is encrypted, the network itself may still be identifiable.

Once a protocol can be reliably identified, blocking it becomes a tractable
problem.

#### A different approach

Nebulon starts with a different premise: **what if there were no single
protocol to identify?**

Rather than attempting to disguise a fixed wire protocol, Nebulon allows each
peer connection to cryptographically derive its own protocol from material
known only to those peers. The resulting protocol space is enormous — roughly
4.2 × 10²² possible combinations — making network-wide protocol
fingerprinting fundamentally different from identifying a conventional
decentralized network.

The objective isn't simply to make classification difficult. It's to make
classification at network scale economically impractical.

#### More than protocol polymorphism

Nebulon is designed as a complete decentralized network rather than a transport
experiment. Its architecture combines:

- **Per-connection polymorphic protocols** derived from shared cryptographic
  material
- **Vivaldi network coordinates** for latency-aware decentralized routing
- **Self-organizing neighborhoods** partitioned using Voronoi-style clustering
- **Epidemic gossip** for decentralized resource discovery and dissemination
- **Peer-elected supernodes** providing logarithmic shortcuts across the network
- **Decentralized naming** without dependence on DNS or a central registrar

The result is a network designed to organize itself, route efficiently, discover
resources, and scale without requiring a central authority or a globally
recognizable protocol.

#### Engineering the network

Nebulon is being developed in **C# / .NET 10** alongside a parallel validation
environment. A discrete-event network simulator is being built to exercise
multi-node behavior, while Python-based algorithmic experiments validate
routing and topology algorithms at scales ranging from hundreds to tens of
thousands of simulated nodes.

The intent is to test the assumptions behind the architecture rather than
simply describe them.

## Why open source?

Silicon Wraith exists as a place to develop and share software openly.

Some projects are new. Others represent ideas and experience accumulated over
years of building distributed platforms, developer infrastructure, and
large-scale software systems. The goal is not simply to publish source code,
but to make the architecture, reasoning, experiments, and lessons behind the
software available as well.

## About the creator

Silicon Wraith was founded by
[John Sheppard](https://github.com/John-Sheppard), a software architect and
engineering leader with a background in distributed systems, scientific
computing platforms, developer infrastructure, and software engineering.

Much of the work here grows out of a long-standing interest in systems that
coordinate across machines — and, increasingly, systems in which software
agents coordinate with each other.

---

**Build interesting things. Understand how they work. Share what you learn.**
