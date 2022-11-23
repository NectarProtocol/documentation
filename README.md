# Introducing: Nectar

Nectar is a publicly accessible, highly scalable, privacy preserving and compliant network that creates a data rich environment for web3 in healthcare.

  

Nectar is an open source protocol built using zero-knowledge rollups and is secured by the Ethereum blockchain. Rollups take processing off the main chain (Layer 1) by computing, storing, and batching transactions off-chain (on Layer 2). This creates a dramatic [100x](https://tim.blog/2021/03/09/vitalik-buterin-naval-ravikant-transcript/) scaling effect compared to L1, enabling more than 4,800 transactions per second for simple transactions. Rollups paired with Ethereum’s future Eth2 sharding increases throughput beyond [100,000](https://vitalik.ca/general/2021/01/05/rollup.html) transactions per second. This high throughput is required in order to meet the existing demand of [82 million](https://www.himss.org/jhim/archive/volume-17-number-1-2003) daily healthcare transactions globally.

  

Despite the healthcare industry’s history of experimenting on private blockchains, Nectar is intentionally secured by Ethereum. Public blockchains, such as Ethereum, provide stronger security, immutability, transparency, [lower costs](https://github.com/EYBlockchain/fundamental-cost-of-ownership/blob/master/EY%20Total%20Cost%20of%20Ownership%20for%20Blockchain%20Solutions.pdf), and the ability to interoperate with other applications as compared to private blockchains. And, rollups have been described as solving the trilemma of public blockchains where there must be a trade off of one of the 3 features: scalability, security, and decentralization. Until now, Ethereum optimized for security and decentralization; with rollups, Ethereum gains robust scalability. No other public blockchains have solved for all 3 ideal characteristics of a public blockchain.

  

Rollup infrastructure is ideal for healthcare (and other industries) where data is required to be highly protected. Rollups can offer the privacy and security required for certain industries such as healthcare, while offering the additional benefit of public blockchains. In order for healthcare to reap the benefits of a public blockchain, the technology must be safe to use and regulatory compliant, which means adhering to existing data privacy and security regulations. In addition to keeping transactions off L1, Nectar accomplishes regulatory compliance in two additional ways:  
  

1.  Privacy Preserving Contracts
    
2.  Authorized Nodes
    

  

The private nature of Nectar comes from the zk-rollup infrastructure and permissions for smart contracts. To regulate access to data contained in smart contracts, we are adding permissions such that contracts can be made private, with access only permitted for pre-specified accounts. Before a user can access a smart contract they will have to prove they are authorized to do so. This change means that composability between contracts can be restricted as needed. It also means that the global state of Nectar's smart contracts are private, and discreetly revealed as needed, for those authorized to see it.

The focus on privacy preservation is what makes Nectar accessible to data-regulated industries as well as individuals whose data is seeding the future of web3.

Authorized Nodes, called Data Service Providers (DSPs), are required to be HIPAA compliant, maintaining certain policies for safe storage and transfer of highly sensitive healthcare data. HIPAA was chosen as the first regulatory requirement in Nectar because it is the most well known, widely used healthcare data privacy regulation globally.

DSPs are authorized to join the network after an authorization and audit, carried out by DSP Authorizers and DSP Auditors. To maintain compliance, DSPs participate in regular audits of HIPAA compliance: passed audits enable DSPs to remain in the network; failed audits kick DSPs out of the network. To discourage fraudulent approvals: DSPs, DSP Authorizers, and DSP Auditors are in a risk-based model with shared revenue and shared data privacy and security breach penalties.

HIPAA compliant DSPs create the distributed data storage infrastructure of Nectar. Private data analytics is a promising, efficient web3 technology and can have a [significant impact](https://www.storj.io/blog/comparing-the-economics-of-centralized-and-decentralized-cloud-storage) on cost savings for healthcare. While individuals and small businesses are likely to adopt distributed data storage before enterprise, the potential for better security, lower cost, and new revenue streams for enterprises will be quite enticing rather than simply shifting an on-prem server to a cloud-based or hybrid cloud system.

Nectar’s unique combination of rollup technology, focus on privacy preservation, and HIPAA compliance creates the needed foundation for the web3 future of healthcare.

  
  
  
  
  

# Nectar Rollup Deep Dive

  

Nectar’s rollup infrastructure is based on zkSync open source code with certain modifications to ensure data privacy compliance. This document assumes that you will access [their exceptional documentation](https://zksync.io) for zkSync-specific detailed technical specifications.

## Why Rollups

  

The purpose of Nectar is to enable the future of healthcare by creating a data rich environment for healthcare’s web3 future. We believe that healthcare innovation is deprived and restricted because of limitations in data access. To bring healthcare innovations to scale, data access is crucial, but so is protecting the individual’s rights to their data.

The future of healthcare becomes a global reality through access to robust data that is owned and governed by the individuals and institutions that created it.

Once a secure, global data web exists, innovation is limitless.

  

We believe that blockchain technology provides the ideal avenue for creating a user-owned, data rich environment for healthcare’s web3.

  

However, blockchains in their current form have flaws that prevent its leading role in the future of healthcare:

  

1.  Slow
    

-   Limited transaction throughput
    

3.  Expensive
    

-   High gas cost for low byte amount
    

5.  Public
    

-   Data and transaction detail is viewable by anyone
    

  

In contrast, healthcare requires technology that is:

1.  Fast
    

-   At least 82 million transactions occur daily in healthcare globally
    

3.  Low cost
    

-   Spending on healthcare is [growing faster](https://www.who.int/health_financing/documents/health-expenditure-report-2019.pdf?ua=1) than the global economy (3.9% and 3.0%, respectively)
    

5.  Private
    

-   Healthcare data has strict privacy regulations, and generally, consumer data privacy laws are becoming more common
    

  

When considering options that work for healthcare’s web3 blockchain infrastructure, Layer 2 technology ticks all the boxes. L2 infrastructure is:

  

1.  Fast
    

-   Improves scalability for public blockchains
    

3.  Low Cost
    

-   Decreases gas cost and congestion
    

5.  Private
    

-   Can enable privacy preservation of smart contracts and data
    

  

There are many Layer 2 options to choose from: State Channels, Plasma, Sidechains, and Rollups. But only the last 2 make sense for healthcare.

  

State Channels and Plasma are ideal for simple transactions, so they are not suitable for healthcare’s complexities (ie:multi-party smart contract execution). And, notably, Optimism [evolved](https://twitter.com/optimismPBC/status/1215410533052055553) from focusing on plasma to rollups.

  

Sidechains and Rollups remain.

  

Sidechain: In 2017, Tamarin developed Health Nexus, our healthcare-specific sidechain (a fork of Ethereum with HIPAA compliant nodes) . Optimizing Health Nexus has been the focus of Tamarin’s National Science Foundation (NSF) $1.2M grant-funded research since 2019. Building a HIPAA-compliant protocol has transformed our team’s understanding of the problems of decentralized tech that are unique to healthcare (and for data privacy in general). Specifically, our NSF research revealed that Health Nexus would not provide the full level of privacy required for healthcare (or other consumer data privacy requirements). This coupled with skyrocketing gas fees and congestion on Ethereum encouraged us to consider alternative options for healthcare’s data web infrastructure.

  

Rollups: While Health Nexus may play a future role as a healthcare-safe sidechain, the goal of creating a compliant way for healthcare to take advantage of the benefits of public blockchains is possible using rollup technology where the data and transactions can be handled privately off-chain.

  

Some may argue that there are L1 blockchains that already offer unmatched speed and low cost, such as Solana, and with ZKP, could also provide privacy preservation. We considered this, but also considered the risks of betting on just one blockchain (i.e.: obsoletion), and that blockchains such as Solana are much younger, less proven, and arguably more centralized than Ethereum.

  

With that, rollups are a better bet than enabling privacy preservation in L1: rollups can be blockchain agnostic, and can make any Layer 1 faster and cheaper. So, securing the rollup with Ethereum is a great starting point; but Nectar is not and will not be limited to one L1. Nectar can bridge to any other blockchain. With rollups we don’t have to bet on just one blockchain. We can enable any blockchain to provide the data privacy required by the healthcare industry.

  

### Optimistic vs. Zero-Knowledge?

  

There are two types of rollups, optimistic and zero-knowledge. They differ technologically in their proofing mechanism, fraud proof vs. validity proof.

  

Fraud proofs are used to challenge the correctness of the state transition.

  

After a thorough code review of optimistic rollups, we eventually settled on ZK-rollups, specifically the zkSync code base.

### Data Service Providers = Nodes

  

In Nectar the biggest difference is that Data Service Providers power the Network and provide HIPAA compliance.

  

Data Service Providers (DSPs) can be individuals or businesses and can serve as Full Nodes, Validators and - roles unique to Nectar - as Authorizers, Auditors, Decentralized Data Providers.

  

DSP Authorizers and DSP Auditors monitor HIPAA compliance for the Network. In the testnet launch of the Network, DSP Authorizers and DSP Auditors will be approved by Nectar representatives. For the mainnet, Nectar will transition to a decentralized approval process of DSP Authorizers and DSP Auditors, mirroring Proof of Authority models.

  

DSP Authorizers assess HIPAA compliance of DSPs and manage the first step for DSPs to join Nectar. DSPs are identifiable and are assessed for HIPAA compliance which includes written policies, training, and data security practices. Nectar will publish HIPAA requirements publicly so any individual or entity has the opportunity to apply as a DSP.

  

The second and last step for DSPs to join Nectar is via a HIPAA audit by a HIPAA Auditor. The DSP can request DSP Auditor services any time after being approved by a DSP Authorizer. The HIPAA Audit confirms that HIPAA compliance has been implemented appropriately. If the audit is passed, the DSP can join the network. If the audit is not passed, the DSP can choose to implement needed changes or not participate in the network. DSP Auditors conduct audits quarterly as required by HIPAA.

  

A key aspect of HIPAA compliance is executing and maintaining [Business Associate Agreements](https://www.hhs.gov/hipaa/for-professionals/covered-entities/index.html). Business Associate Agreements (BAAs) are mandatory agreements between a Covered Entity and a Business Associate (BA).

  

Additionally, if a Business Associate (BA) works with a contractor, and that contractor has access to the BA’s PHI, then the contractor and BA must co-sign a Business Associate Subcontractor Agreement. This ensures that both the BA and Subcontractor are aware of and take steps to ensure the security and safety of the PHI.

  

When DSPs join Nectar, they automatically sign Business Associate and Business Associate Subcontractor Agreements. This process is managed by a smart contract.

  

When DSPs are approved, the HIPAA Auditor will categorize the DSP as a: Covered Entity, Business Associate, or Contractor (i.e.: neither a Covered Entity nor Business Associate, which means the DSP can fulfil the Contractor role) which will trigger the correct BAA for execution. However, BAAs, not BASs, will be required for all DSPs in the same chain when there exists one Covered Entity (CE). This is because of the composability within the chain, and the BA role with a CE.

  

While generally BAAs and BASs have standard content, some parts of the agreement are variable, such as the amount of insurance coverage based on the amount of data under management, and some Covered Entities are strict about the contents of their agreements.

#### Incentivizing HIPAA Compliance

  

In order to ensure proper compliance by DSPs, DSP Authorizers, and DSP Auditors, Nectar has certain controls in place. First, a DSP Authorizer and DSP Auditor cannot be the same individual or entity. The individual or entity can serve as a DSP Authorizer or DSP Auditor, but cannot be both at the same time. This is to prevent a DSP Auditor from auditing a DSP that it had just authorized in a DSP Authorizer role. A DSP Authorizer or DSP Auditor can change its role annually.

  

Second, Nectar has built-in incentives via risk sharing to ensure proper compliance by DSPs, DSP Authorizers, and DSP Auditors. HIPAA breaches are required, per federal law, to be reported and can result in a financial penalty to the DSP. To incentivize and support compliance within the Network, the DSP, DSP Authorizer, and DSP Auditor are in a risk-based arrangement. This means that they share in the upside (revenue) and downside (penalty). The percent of risk sharing is dependent on the role. For example, upside and downside risk is higher for the DSP because the DSP manages the data day to day. The percent of risk sharing is higher for the DSP Auditor than the DSP Authorizer because the DSP Auditor interacts more with the DSP via the initial and quarterly audits. In future versions of Nectar, we aim to allow DSPs, DSP Authorizers, and DSP Auditors to adjust their risk sharing percentage allowing more flexibility and creativity. For example, a DSP Auditor could charge lower up-front fees for a higher percent of upside and downside risk sharing. This risk-based arrangement also opens the opportunity for a decentralized insurance model within Nectar.

  

## Technical Modifications

  

### Network Improvements

To enable a privacy preserving network some changes are necessary.

  

**Governance**  

The Nectar network relies on authorized DSPs requiring on-chain governance to maintain the network. Modifications to the Nectar client and on-chain contracts are required to facilitate this governance. The governance structure and details are not specified in this document, but the goal is to start out centralized and move towards decentrality over time.

  

**Pre-authorized Nodes**  

The validator network consists of HIPAA-compliant DSPs which are contractually obligated to handle data in accordance with security rules as stipulated by federal regulations. These DSPs are legal entities that have executed BAA agreements on-chain, allowing us to associate specific blockchain accounts to these legal entities. To facilitate our privacy-preserving compliant network, modifications need to be made that prevent unauthorized nodes fulfilling the role of a DSPs. Network traffic between DSPs and from the Nectar client will only be permitted between approved entities.

### Privacy-Preserving Smart Contracts

To enable privacy preserving contracts some changes to the way transactions are called, smart contracts are accessed, and data is made available are required.  
  
**Permissions for Smart Contracts**  

To regulate access to data contained in smart contracts we are adding permissions such that contracts can be made private, with access only permitted for pre-specified accounts. Before a user can access a smart contract they will have to prove they are authorized to do so. This change means that composability between contracts can be restricted as needed. It also means that the global state of Nectar's smart contracts are private, and discreetly revealed as needed, for those authorized to see it.

  

**Private Smart Contract Invocation**  

To invoke a smart contract, a signed request is made to access the contract (and any composed contracts). Once authorized, a user is free to interact with the contract. A transaction is created locally, and submitted securely to the DSP network. A transaction receipt along with the hash of the pre and post contract state is sent to the aggregator to include in a batch. On Nectar the aggregator is a public function that can be done by anyone, since an aggregator can always create a batch from a single transaction, Nectar inherits the same censorship resistance as Ethereum.  
  
After aggregating and sequencing the transaction is processed by the DSPs, and a result is created for inclusion into the next rollup block.

  

### L2 Improvements

To enable decentralized data and future data services, some changes are required in the rollup contracts and new interfaces made available at the smart contract level.

  

**Extensible Rollup Blocks**

In order to provide future networks of DSPs that selectively offer varying decentralized services, Nectar’s roll-up blocks belong to a unique network that defines the type of services and the state hashes of the resources those services provide. Two networks are planned at the start, a decentralized storage network that secures files in regulatory compliant data stores, and compliant smart-contract services. As future technology emerges new data services will be able to create a unique chain of Nectar blocks for those services.  
  
**Decentralized Data Storage Service**

The previous modifications were aimed at securing smart contracts state and execution. With this change we’re extending the ability of smart contracts to interact with external decentralized data. This is accomplished by creating a separate network of authorized DSP nodes that manage decentralized data storage. DSPs provide data storage using regulatory compliant data storage, and securing access to the data by deploying a data handling contract on the smart contract network. These DSP-deployed data storage contracts contain relevant meta-data and permissions as well as methods for accessing the data and meta-data.

  

Smart contracts with permission to interact with the data-storage contract will be able to access the meta-data and reason about the properties of the data including: type, availability, and access.

  
Data access is provided through interacting with the data-storage contract. The system is designed such that different types of data may have their own data-storage contract that provide additional interface options.
Nectar Roadmap

  

While we are able to stand on the shoulders of giants (🙏🙌 Open Source Community) there is quite a bit of re-tooling needed to make this adoptable by data-regulated industries such as healthcare.

  

Concluding Remarks  
With Nectar we aim to enable Ethereum for data-regulated industries, starting with HIPAA and protected health information. To do this we’re proposing the use of authorized nodes, private contract execution, and a privacy-preserving zero-knowledge validity proofs.  
  
The ability to responsibly use decentralized technology with private health information will enable healthcare innovations that can improve the quality and availability of healthcare, as well as enable a patient-centric approach to private health data.
