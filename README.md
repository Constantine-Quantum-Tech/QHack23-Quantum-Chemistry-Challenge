# CQTech : QHack 2023's Quantum Chemistry Challenge

For this challenge, we want to use the best of two papers that dealt with the BeH2 molecule: [Kandala et al. (2017)](https://www.nature.com/articles/nature23879) which proposes a reduced parity encoding of BeH2's Hamiltonian, and [Lolur et al. (2023)](https://pubs.acs.org/doi/pdf/10.1021/acs.jctc.2c00807) which proposes a novel error mitigation technique, the Reference state Error Mitigation, alongside other error mitigation tools that Qiskit provide.

An initial implementation of [Kandala et al.](https://www.nature.com/articles/nature23879)'s work in Qiskit provided in this repo. The final submission should cover all of the following points:

* Try 2 Hamiltonian encoding approaches and compare them:
  1. Implement the reduced parity encoding of the Hamiltonian from [Kandala et al. (2017)](https://www.nature.com/articles/nature23879) which needs 6 qubits.
  2. Use Qiskit's tools + Circuit Knitting Toolbox to handle encodings that require a large number of qubits.

* Ansatz:
  * Use Hardware efficient ansätze for both methods.

* Use REM method from [Lolur et al. (2023)](https://pubs.acs.org/doi/pdf/10.1021/acs.jctc.2c00807).
* Use the error mitigation methods provided in Qiksit alongside REM, similarly to Lolur et al..
* Using the 7 qubits devices from IBM may give different accuracies than Kandala et al. due to the different devices topologies. The 16 qubits devices are more useful to reproduce Kandala et al.'s results, since we can use 6 qubits that are linearly connected.
* Finally, analyze all of the obtained results.

**Note:** In Lolur et al., the VQE for BeH2 was only simulated, so our solution may be the first to use their REM on a real device for that molecule.


