# Formal Verification of TEEP Protocol with SUIT Encrypted Payload using ProVerif & Tamarin Prover
The purpose of this project is the formal verification of TEEP protocol with SUIT encrypted payload using ProVerif & Tamarin Prover.
ProVerif & Tamarin Prover is the formal verification tools to analyze the security properties of security protocols.
## What is verified here?
- (DONE)
  - The authentication of TEEPAgent is verified.
  - The secrecy of encrypted payload is verified.
- (TODO)
  - The authentication of TAM is in progress, because our present verification code doesn't deal with TAM Attestation Result and Access Control List [TBD].

## Usage
- See [proverif](https://bblanche.gitlabpages.inria.fr/proverif/)
- See [tamarin_prover](https://tamarin-prover.github.io/)
```
$ proverif TEEP_20231003_13_1.pv
$ tamarin-prover --prove TEEP_20231003_16_1.spthy
```
## LICENSE
See [LICENSE](NTTSoftwareLicenseAgreement_TEEP_20231006.pdf)