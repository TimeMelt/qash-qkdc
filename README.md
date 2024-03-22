<p align='center'><img src="img/qash.png" width="250"></p>

# Qash-QKDC
## Quantum Key-Derivation/Hashing Circuits (Superconductor and Photonic QPUs)
- This jupyter notebook demonstrates a proof of concept for using quantum operations to hash data in a cryptographically secure manner
- There are 2 different circuits demnstrated based on the type of quantum processor (QPU) being used:
  1. superconductor (also compatible with trapped-ion QPUs)
  2. photonic (fock based)
- This notebook uses simulators to demonstrate hashing capabilities, however, these circuits can be ran on physical quantum hardware if adapted correctly
- For proper gaussian-photonic implementation, check out [GausQash](https://github.com/TimeMelt/GausQash)

### Web Demo Now Available!!!
- [![qash-qkdc-ui](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://qkdc-ui.streamlit.app/)
- [web demo source code](https://github.com/TimeMelt/qash-qkdc-streamlit)

### Updates
- specialized gradient calculation
  - less possibility for hash collisions
  - better key-derivation (more possiblities for key/hash outputs)
- new device compatibility:
  - IonQ & AQT (trapped-ion): compatible with superconductor circuit
  - QuTech/Quantum Inspire
  - IBM/Qiskit
  - Google/Cirq
  - Nvidia/CuQuantum
  - Kokkos

#### *Security Note*: these circuits are not battle tested in any capacity and therefore unverified to be cryptographically secure, or programmatically useful in any manner
- If anyone wants to benchmark and/or pentest these circuits feel free to do so
- any feedback related to improving these circuits security and/or usability is highly appreciated

#### General Notes:
- this notebook was created using python v3.11
- These circuits are not particularly fast in runtime (due to the nature of computations being executed)
- in order to help with the preformance drag and to allow execution on different device types, the JAX python library is used
- at the moment these circuits do not work with complex number operations, they do work with single and double-precision float values

#### Future Goals:
- create circuits compatible with neutral-atom QPUs
- continue research/development of new and current circuits using physical quantum hardware (whether through the cloud or on-premise access)
- ~~develop web ui for demo usage!~~

#### Donations (optional):
- Any donation, no matter how small, is greatly appreciated!! 
- [click here to donate](https://buy.stripe.com/fZe4i46ht5mEfMkeUY)

#### Citation (this project):
- please cite this project/repo if using it in research and/or development (USE IN RESEARCH/DEVELOPMENT IS ENCOURAGED)

#### Credits:
- quantum libraries provided by [PennyLane](https://github.com/PennyLaneAI/pennylane): 
  - [pennylane research paper](https://arxiv.org/abs/1811.04968): 

    > Ville Bergholm et al. *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018. arXiv:1811.04968

- accerlation through [JAX](https://github.com/google/jax) library: 
  > jax2018github,
  > author = {James Bradbury and Roy Frostig and Peter Hawkins and Matthew James Johnson and Chris Leary and Dougal Maclaurin and George Necula and Adam Paszke and Jake Vander{P}las and Skye Wanderman-{M}ilne and Qiao Zhang},
  > title = {{JAX}: composable transformations of {P}ython+{N}um{P}y programs},
  > url = {http://github.com/google/jax},
  > version = {0.3.13},
  > year = {2018},
