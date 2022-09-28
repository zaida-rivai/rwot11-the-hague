# A specification for ledger-agnostic AnonCreds

## Abstract

AnonCreds are a novel means of providing digitally verifiable data that is privacy-preserving and tamper-proof (for SSI). Currently, AnonCreds are coupled to Hyperledger Indy, however the underlying cryptographic logic is based on the Hyperledger Ursa library and henceforth uncoupled to any specific ledger. Many real-world use-cases for SSI implementations come with using multiple and different types of ledgers for the same user domain. For instance, a country could use verifiable credentials based on ledger A for issuing a driving license and certificate of citizenship, whilst using ledger B for banking-related matters. The ability to anchor AnonCreds related objects (schemas, credential definitions, etc..) on theoretically any ledger, is the goal of this proposal. The outcome is an AnonCreds specification describing how to use AnonCreds in a ledger agnostic way, based on the current Hyperledger Indy implementation, with modifications/shortcomings that describe possible extensions and updates to the current speicfication (such as removing the binding to CL signatures, or the revocation scheme).