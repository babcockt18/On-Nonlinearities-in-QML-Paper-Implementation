# On Nonlinearities in QML Paper Implementation

This repository provides implementations of basic nonlinear quantum subroutines proposed in *On nonlinear transformations in quantum computation*, including the Quantum Hadamard Product for element-wise multiplication of quantum states and the Generalized Quantum Transpose for weighted transposition. 

In contrast to the paper which uses Qiskit, these implementations are done using the PennyLane quantum machine learning library, providing an alternative implementation. By advancing techniques to perform nonlinear transformations on quantum states, this research aims to enable more powerful quantum algorithms to impact important domains such as quantum machine learning.

## Paper Reference
Holmes, Z., Coble, N. J., Sornborger, A. T., & Subaşı, Y. (2023). Nonlinear transformations in quantum computation. _Phys. Rev. Res._, 5(1), 013105. [DOI: 10.1103/PhysRevResearch.5.013105](https://link.aps.org/doi/10.1103/PhysRevResearch.5.013105)


## Prerequisites and Installation

## Usage and Examples

Provide instructions on how to use the implementation, including example commands or scripts.

### Example Input
### Example Output

## Code Explanation

### Quantum Hadamard Product (QHP.ipynb)

This Jupyter notebook implements the Quantum Hadamard Product algorithm from the paper "On nonlinear transformations in quantum computation".

The Quantum Hadamard Product takes two input quantum states \$\rho(0)\$ and \$\rho(1)\$ and outputs a weighted state \$\rho(0)\rho(1)\$ where the matrix elements are multiplied element-wise.

#### Key points:

- Implements the circuit shown in Fig. 2 of the paper using PennyLane.
- Can be iterated to take powers of a state, as shown in Fig. 3.
- Convergence analysis shows absolute error remains constant but relative error increases with power.
- Demonstrated with hardware implementation on IBMQ-Bogota.

### Generalized Quantum Transpose (GQT.ipynb)

This Jupyter notebook implements the Generalized Quantum Transpose algorithm from the same paper.

The Generalized Quantum Transpose takes an input state \$\rho\$ and ancilla state \$\sigma\$ and outputs the weighted state \$\sigma\rho^T\$ where \$\rho^T\$ is the transpose of \$\rho\$.

#### Key points:

- Implements the circuit shown in Fig. 4 using PennyLane.
- SWAP operator measurement implemented as shown in Fig. 5.
- Can be used to implement powers of a state, but convergence is slower than direct QHP algorithm.
- Related to quantum teleportation algorithm as discussed in Appendix C of the paper.

The two notebooks demonstrate implementations of key quantum algorithms from the paper for performing nonlinear transformations on quantum states. The PDF provides additional details on the algorithms, theory, and analysis.

## Results and Comparisons

## Contact Information




