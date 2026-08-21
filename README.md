<!-- Header -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1f6feb,100:0d1117&height=140&section=header&text=Md%20Nahid%20Hossain&fontSize=38&fontColor=e6edf3&fontAlignY=55&desc=Blockchain%20%7C%20ML%20Research%20%7C%20Full-Stack%20Engineering&descAlignY=80&descColor=7d8590" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=16&duration=2800&pause=1200&color=58A6FF&center=true&vCenter=true&width=680&lines=7+research+papers+under+review;Blockchain+Provenance+%7C+Post-Quantum+Crypto+%7C+RAG;MERN+%7C+Next.js+%7C+ASP.NET+Core+%7C+Solidity;Final-year+CSE+%40+AUST+%E2%80%94+graduating+soon;Open+to+Research%2C+Full-Stack+and+Web3+roles" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0d1117?style=for-the-badge&logo=linkedin&logoColor=58a6ff&labelColor=161b22)](https://linkedin.com/in/nahid-hossain143)
[![Email](https://img.shields.io/badge/Email-0d1117?style=for-the-badge&logo=gmail&logoColor=a371f7&labelColor=161b22)](mailto:nahidmax26@gmail.com)
[![GitHub](https://img.shields.io/badge/Repos-0d1117?style=for-the-badge&logo=github&logoColor=e6edf3&labelColor=161b22)](https://github.com/nahidhossain143?tab=repositories)
<!-- TODO: add these once you have them — they matter a lot for research roles
[![Google Scholar](https://img.shields.io/badge/Scholar-0d1117?style=for-the-badge&logo=googlescholar&logoColor=58a6ff&labelColor=161b22)](YOUR_SCHOLAR_URL)
[![ORCID](https://img.shields.io/badge/ORCID-0d1117?style=for-the-badge&logo=orcid&logoColor=a3cc39&labelColor=161b22)](YOUR_ORCID_URL)
[![Resume](https://img.shields.io/badge/Resume-0d1117?style=for-the-badge&logo=readdotcv&logoColor=e6edf3&labelColor=161b22)](YOUR_RESUME_URL)
-->

</div>

---

## About Me

```text
Status      →  Final-semester B.Sc. CSE, Ahsanullah University of Science & Technology
Location    →  Dhaka, Bangladesh
Research    →  Blockchain Provenance · Post-Quantum Security · RAG & LLM Evaluation
Thesis      →  TrustStream — Decentralized News Video Verification
Building    →  Ethereum DApps · ASP.NET Core services · Next.js frontends
Available   →  Research assistantships, graduate study, remote & relocation roles
```

Final-year CSE student working at the intersection of **verifiable systems and machine
learning** — cryptographic provenance for media, cross-chain credential infrastructure,
and evaluation methods for retrieval-augmented and agentic LLMs. Seven papers currently
under review. Alongside research, I ship production web and mobile software: REST APIs,
smart contracts, and cross-platform apps.

---

## Research

All seven manuscripts are **under review**. Preprints and code will be linked as they clear review.

### Blockchain, Provenance & Security

**SentinelVeil** — *Decentralized, Post-Quantum Secure Urban Surveillance*
A four-tier platform that ingests multi-camera video at the edge, encrypts and authenticates
it end-to-end with post-quantum cryptography, batches metadata through a zk-SNARK rollup, and
anchors state on-chain. Implemented as three top-level projects in one monorepo.
<!-- TODO: fill in — PQC scheme (Dilithium/Kyber?), proving system, throughput, proof-generation time -->
`Post-Quantum Crypto` · `zk-SNARK Rollup` · `Edge Ingest` · `On-Chain Anchoring`

**TrustStream-Fabric** — *Consortium-Endorsed Provenance and Segment Integrity for C2PA-Aligned Live News Streaming*
Extends segment-level integrity guarantees to **live** streams under a consortium endorsement
model, aligning per-segment provenance with the C2PA specification so tampering is detectable
mid-broadcast rather than after the fact.
<!-- TODO: endorsement latency, segment overhead, TPS, consortium size -->
`Hyperledger Fabric` · `C2PA` · `HLS` · `Live Provenance`

**CCRM** — *A Staleness-Bounded Gossip Protocol for Scalable Cross-Chain Verifiable Credential Revocation*
A gossip protocol that propagates verifiable-credential revocations across heterogeneous chains
with a provable upper bound on staleness — so a revoked credential can never be accepted beyond
a known time window, without requiring global consensus on every revocation.
<!-- TODO: staleness bound, propagation latency, node count, message overhead, chains/DID stack used -->
`Cross-Chain` · `Verifiable Credentials` · `Gossip Protocol` · `Staleness Bounds`

**CPC** — *Causal Provenance Chain*
Blockchain-anchored Proof-of-Cause framework binding PRNU sensor fingerprints, gyroscopic
telemetry, and Dempster–Shafer trust fusion to an immutable ledger.
`~3,247 TPS` · `Sub-second finality` · `TEE secured` · `Hyperledger Fabric`

**SecureEther** — *Ethereum Fraud Detection*
Hybrid PCA-ensemble (Random Forest + XGBoost) with SMOTE balancing and SHAP explainability for
real-time fraud detection. Trains in **6.9s** against a 987s stacking baseline.
`99.8% Accuracy` · `100% ROC-AUC` · `99.5% F1`

### NLP & LLM Evaluation

**Provenance-Oriented Bengali RAG with Cross-Lingual Multi-View Retrieval and Citation Support Analysis**
An end-to-end Bengali RAG pipeline with sentence-level citation enforcement — multi-view
cross-lingual retrieval over Wikipedia passages via FAISS, NLLB-200 translation, Qwen2.5
generation, and mDeBERTa NLI verification — targeting hallucination in low-resource South
Asian language models.
<!-- TODO: confirm whether these carry over from the earlier version or need updating for the multi-view results -->
`BERTScore F1 60.71%` · `83.19% Citation Coverage` · `5.75% Hallucination Rate` · `99.52% NLI Accuracy`

**RIAGE** — *Trajectory-Level Evaluation of Clinical LLM Agents Beyond Final Accuracy*
An evaluation framework that scores clinical LLM agents on the **reasoning trajectory** rather
than final-answer accuracy alone — surfacing unsafe intermediate steps that terminal metrics
reward equally with sound ones.
<!-- TODO: benchmark/dataset, models evaluated, metrics, headline finding -->
`Clinical NLP` · `Agent Evaluation` · `LLM Safety`

---

## Engineering

### 🔗 TrustStream — Decentralized News Video Verification
> B.Sc. Thesis · AUST

Three-layer platform (React · Node.js · Ethereum) where journalists upload MP4s that are
HLS-segmented, SHA-256 chain-hashed, C2PA v2.2 manifested, IPFS-pinned, and registered on
Ethereum Sepolia through a 3-org consortium. Viewers get real-time tamper detection: a hash
mismatch pauses playback, raises a red overlay, and auto-fires an on-chain `reportTamper()`.

![Solidity](https://img.shields.io/badge/Solidity-0d1117?style=flat-square&logo=solidity&logoColor=e6edf3)
![Ethereum](https://img.shields.io/badge/Sepolia-0d1117?style=flat-square&logo=ethereum&logoColor=a371f7)
![IPFS](https://img.shields.io/badge/IPFS-0d1117?style=flat-square&logo=ipfs&logoColor=58a6ff)
![React](https://img.shields.io/badge/React-0d1117?style=flat-square&logo=react&logoColor=58a6ff)
![Node.js](https://img.shields.io/badge/Node.js-0d1117?style=flat-square&logo=node.js&logoColor=3fb950)
![FFmpeg](https://img.shields.io/badge/FFmpeg-0d1117?style=flat-square&logo=ffmpeg&logoColor=3fb950)

`52 unit tests passing` · `Verified on Blockscout & Sourcify` · `C2PA v2.2` · `3-org consortium`

<!-- TODO: add repo link, demo video, deployed URL, and the verified Sepolia contract address -->

<!-- TODO: add 2–3 non-research engineering projects here — an ASP.NET Core service,
     a Flutter app, a Next.js build. Recruiters for full-stack roles look for these
     specifically, and right now this section rests entirely on the thesis. -->

---

## Tech Stack

**Languages**

![TypeScript](https://img.shields.io/badge/TypeScript-0d1117?style=flat-square&logo=typescript&logoColor=3178c6)
![JavaScript](https://img.shields.io/badge/JavaScript-0d1117?style=flat-square&logo=javascript&logoColor=f0db4f)
![Python](https://img.shields.io/badge/Python-0d1117?style=flat-square&logo=python&logoColor=d29922)
![C#](https://img.shields.io/badge/C%23-0d1117?style=flat-square&logo=csharp&logoColor=a371f7)
![Solidity](https://img.shields.io/badge/Solidity-0d1117?style=flat-square&logo=solidity&logoColor=e6edf3)
![Java](https://img.shields.io/badge/Java-0d1117?style=flat-square&logo=openjdk&logoColor=f05340)
![C++](https://img.shields.io/badge/C++-0d1117?style=flat-square&logo=cplusplus&logoColor=58a6ff)
![PHP](https://img.shields.io/badge/PHP-0d1117?style=flat-square&logo=php&logoColor=58a6ff)

**Frontend & Mobile**

![Next.js](https://img.shields.io/badge/Next.js-0d1117?style=flat-square&logo=nextdotjs&logoColor=e6edf3)
![React](https://img.shields.io/badge/React-0d1117?style=flat-square&logo=react&logoColor=58a6ff)
![Flutter](https://img.shields.io/badge/Flutter-0d1117?style=flat-square&logo=flutter&logoColor=58a6ff)
![TailwindCSS](https://img.shields.io/badge/Tailwind-0d1117?style=flat-square&logo=tailwindcss&logoColor=38bdf8)
![Bootstrap](https://img.shields.io/badge/Bootstrap-0d1117?style=flat-square&logo=bootstrap&logoColor=a371f7)

**Backend & Data**

![Node.js](https://img.shields.io/badge/Node.js-0d1117?style=flat-square&logo=node.js&logoColor=3fb950)
![Express](https://img.shields.io/badge/Express-0d1117?style=flat-square&logo=express&logoColor=e6edf3)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET_Core-0d1117?style=flat-square&logo=dotnet&logoColor=a371f7)
![Laravel](https://img.shields.io/badge/Laravel-0d1117?style=flat-square&logo=laravel&logoColor=f05340)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0d1117?style=flat-square&logo=postgresql&logoColor=58a6ff)
![MongoDB](https://img.shields.io/badge/MongoDB-0d1117?style=flat-square&logo=mongodb&logoColor=3fb950)
![MySQL](https://img.shields.io/badge/MySQL-0d1117?style=flat-square&logo=mysql&logoColor=58a6ff)
![Redis](https://img.shields.io/badge/Redis-0d1117?style=flat-square&logo=redis&logoColor=f05340)
![Firebase](https://img.shields.io/badge/Firebase-0d1117?style=flat-square&logo=firebase&logoColor=d29922)

**Blockchain & Web3**

![Ethereum](https://img.shields.io/badge/Ethereum-0d1117?style=flat-square&logo=ethereum&logoColor=a371f7)
![Hardhat](https://img.shields.io/badge/Hardhat-0d1117?style=flat-square&logo=hardhat&logoColor=d29922)
![Foundry](https://img.shields.io/badge/Foundry-0d1117?style=flat-square&logo=foundryvirtualtabletop&logoColor=e6edf3)
![Web3.js](https://img.shields.io/badge/Web3.js-0d1117?style=flat-square&logo=web3dotjs&logoColor=f05340)
![Hyperledger](https://img.shields.io/badge/Hyperledger_Fabric-0d1117?style=flat-square&logo=hyperledger&logoColor=3fb950)
![IPFS](https://img.shields.io/badge/IPFS-0d1117?style=flat-square&logo=ipfs&logoColor=58a6ff)

**ML & Infrastructure**

![HuggingFace](https://img.shields.io/badge/HuggingFace-0d1117?style=flat-square&logo=huggingface&logoColor=d29922)
![scikit-learn](https://img.shields.io/badge/scikit--learn-0d1117?style=flat-square&logo=scikit-learn&logoColor=f05340)
![XGBoost](https://img.shields.io/badge/XGBoost-0d1117?style=flat-square&logo=xgboost&logoColor=a371f7)
![FAISS](https://img.shields.io/badge/FAISS-0d1117?style=flat-square&logo=meta&logoColor=58a6ff)
![Docker](https://img.shields.io/badge/Docker-0d1117?style=flat-square&logo=docker&logoColor=58a6ff)
![AWS](https://img.shields.io/badge/AWS-0d1117?style=flat-square&logo=amazonwebservices&logoColor=d29922)

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1f6feb,100:0d1117&height=100&section=footer" />

*Dhaka, Bangladesh · Blockchain & ML Researcher · Open to remote & relocation*

</div>
