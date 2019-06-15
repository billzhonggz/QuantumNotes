# Quantum Computation

Qubits and quantum gates.

## Single Qubit Gates

> Reference: section 1.3.1, *Quantum Computation and Quantum Information*.

Like a normal bit and gate, we start from the `NOT` gate. The truth table for a `NOT` gate in a normal bit will be easy, just 0 -> 1, and 1 -> 0.

For a quantum bit, a `NOT` gate will be a *linear* space like $\alpha|1> + \beta|0>$, comes from the original representation of $\alpha|0> + \beta|1>$.

For historical reason, a quantum `NOT` gate is defined as $X$.

$
X \equiv 
\begin{bmatrix}
0 & 1\\
1 & 0\\
\end{bmatrix}
$

Then we can get,

$X
\begin{bmatrix}
\alpha \\
\beta \\
\end{bmatrix} =
\begin{bmatrix}
\beta \\
\alpha \\
\end{bmatrix}
$

Any *unitary matrix* can form a valid quantum gate. And also, there are two important gates, the $Z$ gate and $H$ (*Hadamard*) gate.

$
Z \equiv
\begin{bmatrix}
1 & 0\\
0 & -1\\
\end{bmatrix},
H \equiv \frac{1}{\sqrt{2}}
\begin{bmatrix}
1 & 1\\
1 & -1\\
\end{bmatrix}
$

## Multi-Qubits Gates

> Reference: section 1.3.2, *Quantum Computation and Quantum Information*.

At this section, `AND`, `OR`, `XOR`, `NAND`, and `NOR` gates will be discussed.

A *prototypical* multi-qubit quantum logic gate is the **controlled-`NOT`** (`CNOT`) gate.

### Controlled-NOT gate

A `CNOT` gate takes two qubits as input. One is control qubit and another is target qubit.

$
U_{CN}=\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 \\
\end{bmatrix}
$

## Quantum Algorithms

> Reference: section 1.4, *Quantum Computation and Quantum Information*.

Like the classical computers, quantum computers should have their own set of algorithms. These algorithms should adapt to the preferences of quantum computers.

### Classical computations on quantum computers

To stimulate classical computations on quantum computer, one thing we need is [*Toffoli gates*](https://en.wikipedia.org/wiki/Toffoli_gate). A Toffoli gate can stimulate gates in classical computers. Since it can provide **deterministic** computation results.

Quantum computers can also stimulate *non-deterministic* classic computers.

### Quantum parallelism

*Quantum parallelism* is a fundamental feature for many quantum algorithms.
