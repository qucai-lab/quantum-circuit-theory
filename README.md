<!-- Badges: -->
[![Python](https://img.shields.io/badge/Python-3.11.2-informational)](https://www.python.org/)
[![Contributions](https://img.shields.io/badge/contributions-welcome-orange?style=flat-square)](https://github.com/qucai-lab/quantum-circuit-theory/pulls)
[![License](https://img.shields.io/github/license/QuCAI-Lab/quantum-circuit-theory.svg?logo=CreativeCommons&style=flat-square)](https://github.com/qucai-lab/quantum-circuit-theory/blob/main/LICENSE.md)

<!-- Logo: -->
<div align="center">
  <a href="https://qucai-lab.github.io/">
    <img src="https://github.com/qucai-lab/qucai-lab.github.io/blob/main/assets/QuCAI-Lab.png" height="500" width="500" alt="Logo">
  </a>
</div>

<!-- Title: -->
<div align="center"> 
  <h1> Quantum Circuit Theory and Implementations </h1>
</div>

<!-- Dependencies: -->
# Dependencies
<a href="https://www.python.org/" target="_blank" rel="noopener noreferrer"><img height="27" src="https://www.python.org/static/img/python-logo.png"></a>
<a href="https://matplotlib.org" target="_blank" rel="noopener noreferrer"><img height="27" src="https://matplotlib.org/_static/images/logo2.svg"></a>
<a href="https://numpy.org/" target="_blank" rel="noopener noreferrer"><img height="27" src="https://numpy.org/images/logo.svg"></a>
<a href="https://sympy.org/" target="_blank" rel="noopener noreferrer"><img height="27" src="https://www.sympy.org/static/images/logo.png"></a>
<a href="https://scipy.org/" target="_blank" rel="noopener noreferrer"><img height="27" src="https://scipy.org/images/logo.svg"></a>
<a href="https://qiskit.org/" target="_blank" rel="noopener noreferrer"><img height="27" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Qiskit-Logo.svg/1200px-Qiskit-Logo.svg.png"></a>

<br>

# Table of Contents

- **[00_formalism](notebooks/00_formalism.ipynb)**
	- Linear operators
	- Outer product representation
	- Basis states
		- Z-basis
		- X-basis
		- Y-basis
	- Pauli group
		- Pauli gates
		- Pauli algebra
	- Clifford group
		- Clifford gates
	- Hermitian gates
	- Spectral decomposition theorem
	- Operator function
- **[01_postulates](notebooks/01_postulates.ipynb)**
	- Dirac notation
	- Postulate 1 (State Space)
		- First case: discrete spectrum
		- Second case: continuous spectrum
	- Postulate 2 (Evolution)
	- Postulate 3 (Measurement)
		- Projective measurement (a.k.a von Neumann measurement) and Born's rule
		- Expectation value
	- Postulate 4 (Composite State)
	- System's Dynamics: Schrödinger equation
		- Wave Mechanics formalism
	 	- Matrix Mechanics formalism
			- Schrödinger Picture (S-P)
			- Heisenberg Picture (H-P)
	- Solution to the Schrödinger equation
- **[02_single_qubit_gates](notebooks/02_single_qubit_gates.ipynb)**
	- Pauli gates.
	- Hadamard gate a.k.a superposition gate
	- $R_{\hat{n}}(\theta)$ standard rotation single-qubit gate
	- $P(\lambda)$ single-qubit phase gate
		- Phase gate S
		- Phase gate T
	- $U(\alpha, \beta, \gamma, \delta)$ arbitrary single-qubit gate
	- $U(\theta, \phi, \lambda)$ three-parameter single-qubit gate
	- Qiskit $U1(\lambda)\equiv U(0,0,\lambda)=P(\lambda)$
	- Qiskit $U2(\phi, \lambda) \equiv U(\pi/2, \phi, \lambda)$
- **[03_two_qubit_gates](notebooks/03_two_qubit_gates.ipynb)**
- Deriving gates via spectral theorem, parity trick, and single-qubit rotations
	- CNOT gate
	- SWAP gate
	- $ZZ(t)$ gate
	- $XX(t)$ gate
	- $YY(t)$ gate
	- Verifying outer products
- **[04_multi_qubit_gates](notebooks/04_multi_qubit_gates.ipynb)**
	- Multi-qubit gate $C_n^{j}(U_{2^m})$ with $n$ control qubits and $m$ target qubits
- **[05_gate_circuit_identities](notebooks/05_gate_circuit_identities.ipynb)**
	- Qiskit little-endian convention
	- Pauli gates
	- Single-qubit gates
	- Multi-qubit gates
		- Phase Kickback
	- Rotations
	- Conjugation by Unitary
- **[06_gate_decomposition](notebooks/06_gate_decomposition.ipynb)**
	- Pauli decomposition
	- Single-qubit gate decomposition
	- Two-qubit gate decomposition
- **[07_universal_gate_set](notebooks/07_universal_gate_set.ipynb)**
	- Obtaining the universal gate set
- **[08_change_of_basis](notebooks/08_change_of_basis.ipynb)**
	- From the $Z$-basis to the $X$-basis
	- From the $Z$-basis to the $Y$-basis
	- Quantum circuits for measurement in a different basis
		- Measurement in the $𝑍$-basis
		- Measurement in the $X$-basis
		- Measurement in the $Y$-basis
- **[09_state_preparation](notebooks/09_state_preparation.ipynb)**
 	- Introduction
	- Unitary Decomposition 
	- Schmidt Decomposition 
	- Qiskit Examples
- **[10_trotterization](notebooks/10_trotterization.ipynb)**
	- The Trotter-Susuki formula
	- The Heisenberg XXX Spin-1/2 Lattice Model for $N=3$ Three Particles
	- Decomposition of $U_{\text{Heis3}}(t)$ using Trotterization
	- About the Trotterized Evolution
	    - Verifying identities with NumPy
	    - Verifying identities with Qiskit Opflow
- **[11_implementations](notebooks/11_implementations.ipynb)**
	- NumPy and Sympy implementations of:
		- Basis states.
		- Projector operators.
		- Single-qubit gates.
		- Two-qubit gates.
		- Eigenvalues and eigenvectors.
- **[12_algebraic_identities](notebooks/12_algebraic_identities.ipynb)**
	- Notation.
	- Representations.
	- Identities: algebraic proof of useful linear algebra identities for quantum circuits with SymPy and SciPy verification.
		- Retangular matrices.
		- Vectors.
		- Kronecker product between vectors.
		- Kronecker product between retangular matrices.
		- Kronecker product with vectors and matrices.
		- Commutation.
		- Matrix exponential.
		- Rotations.
- **[13_glossary](notebooks/13_glossary.ipynb)**
	- Jargon and Terminology.
- **[14_Q&A](notebooks/14_Q.ipynb)**
	- Questions and Answers.
  
# Conda Env.

1. Clone this repository and access the cloned directory:
```bash
git clone https://github.com/qucai-lab/quantum-circuit-theory.git && cd quantum-circuit-theory
```
2. Create env.:
```bash
conda create -yn qct python==3.11.2 && conda activate qct
```
3. Install core dependencies:
```
python -m pip install -r requirements.txt
```

# References &nbsp; <a href="#"><img valign="middle" height="45px" src="https://img.icons8.com/book" width="45" hspace="0px" vspace="0px"></a> 

\[1] Nielsen MA, Chuang IL. 2010. "Quantum Computation and Quantum Information." New York: [Cambridge Univ. Press.](https://doi.org/10.1017/CBO9780511976667) 10th Anniv. Ed. 
- Corollary 4.2, pg. 176: Gate decomposition.
- Theorem 4.3, pg. 207: Trotter formula. 
- Chapter 4.7.2, pg. 206: The quantum simulation algorithm. 

\[2] Barenco, A., Bennett, C.H., Cleve, R., DiVincenzo, D.P., Margolus, N., Shor, P., Sleator, T., Smolin, J.A. and Weinfurter, H. (1995) Elementary gates for quantum computation. [Phys. Rev. A 52, 3457–3467](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.52.3457).

\[3] Scott Aaronson and Daniel Gottesman. 2004. Improved simulation of stabilizer circuits. [Phys. Rev. A 70, 5](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.70.052328) (Nov. 2004),
052328.

\[4] John Preskill. "Course Information for Physics 219/Computer Science 219 Quantum Computation." [California Institute of Technology](http://theory.caltech.edu/~preskill/ph229/).
- Chapter 5: Classical and Quantum Circuits.

\[5] Hans J. Weber and George B. Arfken. Essential Mathematical Methods for Physicists. [Academic Press, NY](https://g.co/kgs/RFBRhf).

# License

This work is licensed under a [Creative Commons Zero v1.0 Universal](LICENSE.md) license.

<hr>
