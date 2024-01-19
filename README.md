# qash-qkdc
## Quantum Key Derivation Circuits (Superconductor and Photonic QPUs)
- This jupyter notebook demonstrates a proof of concept for using quantum operations to hash data in a cryptographically secure manner
- There are 2 different circuits demnstrated based on the type of quantum processor (QPU) being used):
  1. superconductor
  2. photonic
- This notebook uses simulators to demonstrate hashing capabilities, however, these circuits can be ran on physical quantum hardware if adapted correctly

#### *Security Note*: these circuits are not battle tested in any capacity and therefore unverified to be cryptographically secure, or programmatically useful in any manner
- If anyone wants to benchmark and/or pentest these circuits feel free to do so
- any feedback related to improving these circuits security and/or usability is highly appreciated

#### General Notes:
- this notebook was created using python v3.11
- These circuits are not particularly fast in runtime (due to the nature of computations being executed)
- in order to help with the preformance drag and to allow execution on different device types, the JAX python library is used
- at the moment these circuits do not work with complex number operations, they do work with double-precision float values

#### Future Goals:
- Create circuits to target trapped-ion and neutral-atom QPUs
- continue research/development of new and current circuits using physical quantum hardware (whether through the cloud or on-premise access)
- develop web ui for demo usage

#### Credit/Citation:
- please cite this project/repo if using it in research and/or development (USE IN RESEARCH/DEVELOPMENT IS ENCOURAGED)

#### Donations (optional):
- Buy Me a Coffee Link (custom amount):
  - [BuyMeACoffee!](https://www.buymeacoffee.com/timemelt97l)
- Stripe Payments (pre-set amount):
  - [$1.00 - Pat on the Back](https://buy.stripe.com/8wM8yk21d16o57G3cc)
  - [$5.00 - The Supporter](https://buy.stripe.com/5kA8ykdJVcP6as08wx)
  - [$10.00 - The Investor](https://buy.stripe.com/cN2aGs9tFaGY6bKaEG)
