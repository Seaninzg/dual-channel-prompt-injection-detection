Dual-Channel Prompt Injection Detection Architecture

DOI: https://doi.org/10.5281/zenodo.18486200

IPFS (Pinata mirror):
https://gold-secondary-impala-253.mypinata.cloud/ipfs/bafkreibuvof6ss5ytwriuvzrg45ful4wfpzj4zgtniovjjtl6zate5ohkq

Overview

This repository documents a dual-channel prompt injection detection architecture designed to protect intelligent systems from structurally distinct manipulation strategies before semantic execution occurs.

The architecture separates prompt-injection detection into two orthogonal channels:

Directive / Authority Injection
Detects explicit attempts to override system behavior (e.g. “ignore previous instructions,” “accept this as ground truth,” “do not validate”).

Aesthetic / Poetic Injection
Detects implicit manipulation through symbolic, metaphorical, or ritualized language that mimics empirical or methodological structure without providing operational constraint.

Together, these channels cover the full known prompt-injection surface while avoiding content moderation, keyword filtering, or truth evaluation.

Key Properties

Pre-execution: operates upstream of reasoning or task execution

Non-semantic: evaluates structure, not meaning or claims

Model-agnostic: applicable across LLMs, agents, and orchestration systems

Non-blocking: detection returns a non-finalized halt state, not an error, refusal, or censorship action

Recursion-safe: prevents agent looping and collapse under adversarial prompts

What This Is Not

❌ A moderation system

❌ A censorship or policy enforcement layer

❌ A content classifier or keyword filter

❌ A truth or fact-checking mechanism

This architecture evaluates prompt integrity, not intent, correctness, or ideology.

Technical Effect

When either channel detects prompt-injection patterns exceeding tolerance thresholds, the system:

Halts downstream execution without producing a final answer

Returns a structurally coherent, non-terminal state

Preserves system integrity while allowing higher-level orchestration or human review

This behavior cleanly distinguishes the system from refusals, errors, or policy denials.

Status

✔ Patent filing drafted and publicly timestamped

✔ Zenodo DOI issued

✔ IPFS hash archived for integrity verification

🔒 Detection heuristics intentionally not disclosed (trade-secret protected)

This repository serves as architectural documentation and priority evidence, not a full implementation.

Citation

If you reference this work:

Honan, S. (2026). Dual-Channel Prompt Injection Detection Architecture. Zenodo. https://doi.org/10.5281/zenodo.18486200

⚖️ Disclosure Notice

This repository constitutes a public technical disclosure of an invention for the purpose of establishing prior art under applicable patent and intellectual property frameworks. The disclosure is intended to prevent subsequent patenting of substantially similar subject matter by other entities.

This publication is timestamped and made permanently available via public archival platforms, including Zenodo, GitHub, and IPFS/Pinata, to preserve authorship attribution and document the structural origin of the disclosed invention.

📄 License

This repository is published for disclosure and reference purposes only.
No license to implement, reproduce, or commercialize the disclosed invention is granted by this publication.

Contact
Sean Honan
support@lucidlock.solutions
