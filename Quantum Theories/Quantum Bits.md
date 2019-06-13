# Quantum Bits

Quantum bits (qubits) are the base of a quantum system.

## A Quantum Bit

> Reference: section 1.2, *Quantum Computation and Quantum Information*.

Like the *bit* we know from information theory, a quantum bit have two *basic* states, |0> and |1>. The difference between a `bit` and a `qubit` is a `qubit` can be in a state *other* than |0> and |1>. It is also possible to form *linear combinations* of states, often called *superpositions*.

$|\psi> = \alpha|0> + \beta|1>$

Notation `|>`, is called the *Dirac notation*, the standard notation for states in quantum mechanics.

### States of one qubit

The states `|0>` and `|1>` are known as *computational basis states*, and form an **orthonormal basis** for this vector space.

In general, a qubit's state is a unit vector in a two-dimensional complex vector space.

Finally, the states of a qubit can locates in a *Bloch sphere*.

### Information contains by a qubit

- There are an infinite number of points in a unit sphere.

## Multiple Quantum Bits

> Reference: section 1.3, *Quantum Computation and Quantum Information*.

According to the equation above, two qubits can have the state vector like,

$|\psi> = a_{00}|00> + a_{01}|01> + a_{10}|10> + a_{11}|11>$

### Measuring subsets

For the system of two qubits, the subset of it should be a system has only one qubit. For this system, we can measure just one subset of it.

Giving 0 with probability $|a_{00}|^2 + |a_{01}|^2$, and leaving the **post-measurements**,

<!-- TODO: Understand the normalization stuff. -->

$|\psi'> = \frac{a_{00}|00> + a_{01}|01>}{\sqrt{|a_{00}|^2 + |a_{01}|^2}}$.

An important two qubits state is the *Bell state* or *EPR pair*,

$\frac{|00> + |11>}{\sqrt{2}}$.

### Measuring $n$ qubits

Compute the basis states of the system are of the form $|x_{1}x_{2}...x_{n}>$, and a quantum state for such a system is specified by $2^n$ amplitudes.