# Training for Formal Verification of TEEP Protocol with SUIT Encrypted Payload using ProVerif & Tamarin Prover
The purpose of this project is the training for the formal verification of TEEP protocol with SUIT encrypted payload using ProVerif & Tamarin Prover.
ProVerif & Tamarin Prover is the formal verification tools to analyze the security properties of security protocols.
- (TODO)
  - The authentication of TEEPAgent is in progress.
  - The secrecy of encrypted payload is in progress.
  - The authentication of TAM is in progress, because our present verification code doesn't deal with TAM Attestation Result and Access Control List [TBD].

(2024/02/14)
- I revised my code thoroughly based on the draft below,
  A Usable Formal Methods Sample Problem from TEEP
  (https://datatracker.ietf.org/doc/draft-mt-ufmrg-teep-sample/).
  Specifically, I thought this draft is based on "background check model",
  and fixed the entities and the security properties in my code accordingly.
- I addressed the issue according to the advice in IETF118.
  Specifically, I fixed the protocol and the communication channel 
  which is not likely to cause the result "cannot be proved".

I hope this code to be treated as an instance of the draft above.

## Usage
- See [proverif](https://bblanche.gitlabpages.inria.fr/proverif/)
```
$ proverif TEEP_20240214_34.pv
```
- See [tamarin_prover](https://tamarin-prover.github.io/)
```
$ tamarin-prover --prove TEEP_20231003_16_1.spthy
```
## LICENSE
See [LICENSE](NTTSoftwareLicenseAgreement_TEEP_20231006.pdf)
