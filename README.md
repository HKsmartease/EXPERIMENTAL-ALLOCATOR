# FLOW Model: DataCap Allocation Evaluation Criteria

**FLOW: An Innovative Evaluation Framework for Filecoin+ Experimental Allocators**

This framework provides a simple, transparent, and automated evaluation system for experimental allocators in the Filecoin+ project. The goal is to lower entry barriers, foster innovation, and ensure responsible resource utilization.

## Objectives

- Reduce barriers for experimental allocator participation
- Provide quantitative and transparent evaluation criteria
- Utilize on-chain data for verifiable tracking
- Prevent abuse and encourage successful transition to standard allocation paths

## Scoring Formula

**Final Score = Utilization × Success Rate × Type Weighting Factor**

| Symbol | Description |
| --- | --- |
| S | Final Score |
| U | Utilization |
| Q | Success Rate |
| T | Type Weighting Factor |

### Key Metrics Definition

#### 1. Utilization (U)

**U = Used DC / Allocated DC**

- **Source**: On-chain consumption data from the past 30 days

#### 2. Success Rate (Q)

**Q = Successful Transactions / Total Transactions**

- **Source**: On-chain storage transaction status
- **Note**: Excludes slashed or expired transactions

#### 3. Type Weighting Factor (T)

| Data Type | Weighting Factor (T) |
| --- | --- |
| Public/Non-profit/Research | 1.5 |
| Web3 Infrastructure/Education | 1.3 |
| Commercial/Private Storage | 1.0 |

## Allocation Logic

**Monthly Evaluation**

1. All applicants are ranked by score (S).
2. High-scoring applicants are prioritized for DataCap allocation.
3. Applicants with scores below the threshold (e.g., S &lt; 0.4) may have allocations paused.
4. Allocation results and scores are publicly recorded, stored on-chain or on IPFS.

## Risk and Penalty Policy

| Condition | Consequence |
| --- | --- |
| U &lt; 0.4 for two consecutive months | Allocation paused |
| Q &lt; 0.6 or detected fraudulent transactions | Review or disqualification |
| Misreporting data type to abuse weighting factor (T) | Permanent disqualification |

## Use Cases

- Evaluate DataCap applicants for experimental allocators
- Support EPMA pathways, ensuring quantifiable and verifiable data
- Scalable, integrating GitHub activity or KYC levels
