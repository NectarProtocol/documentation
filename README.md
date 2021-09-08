# Nectar Protocol


# Introduction


In 2014, the [Living Heart Project](https://www.3ds.com/products-services/simulia/solutions/life-sciences-healthcare/the-living-heart-project/) kicked off, debuting the first simulated real-life heart. Powered by the 3DExperience platform from Dassault Systèmes, the research has brought together leading physicians, researchers, educators, medical device developers, regulatory agencies, and practicing cardiologists from across the world to develop personalized digital heart models. The project just received additional federal funding, expanding the scope to virtual patients and computational modeling.

  

In 2017, an article in The Journal of Arthroplasty found that [personalized knee replacement](https://www.arthroplastytoday.org/article/S2352-3441(17)30040-7/fulltext) devices had far better outcomes at no additional cost than “out of the box” knee replacement devices.

  

In 2018, a [study](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6202760/) was published in Acta Orthopaedica about a December 2017 shoulder replacement surgery on an 80-year old woman with advanced arthritis. This surgery was guided by Microsoft’s HoloLens, which personalized guided steps for the surgery based on the patient’s medical history and operating technique which were accessible and visible in real time via the HoloLens: “the surgeon was able to compare, stage by stage, what he was doing with what had to be done” for the surgery.

  

In 2019, a surgeon in China successfully completed a liver removal of a lab animal over a 5G internet connection. The surgeon was at a different location [30 miles away](https://in.pcmag.com/news/128092/china-performs-first-5g-remote-surgery).

  

In 2020, because of the COVID-19 Pandemic, clinicians in the United States were allowed to practice telemedicine [across state borders](https://www.hhs.gov/coronavirus/telehealth/index.html) without concern for their State Licensure. In 2021, the Center for Care Innovations presented a host of evidence that, for many clinical applications, telemedicine was [just as if not more effective](https://www.careinnovations.org/virtualcare/resources/evidence-for-telemedicine-efficacy-and-quality/) than in-person care.

  

In 2021, the opportunity of in silico trials promises [better, faster, and cheaper clinical trials](https://trialsjournal.biomedcentral.com/articles/10.1186/s13063-020-05002-w) by assessing potential drug and therapy impact via computer simulation and large datasets.

  

The future of healthcare is exciting. The future of healthcare is Web3.

  

The future of healthcare is not bound by geographical boundaries; it blurs the line between reality and digital; it is more effective and less expensive; it is data rich.

  

The key to Web3 for healthcare is personalized medicine which is made possible by personalized, identifiable data.

  

This elevates the importance and necessity of data in Web3. It also means that “ethical issues related to fair and responsible data usage, as well as [privacy, ownership, security, and authentication](https://www2.deloitte.com/us/en/insights/topics/digital-transformation/web-3-0-technologies-in-business.html) are paramount.”

  

Using healthcare data is a bit more challenging because of the strict data and security regulations specifically for personally identifiable data. And, in general, with the [growing concern](https://www.internetsociety.org/resources/doc/2019/trust-opportunity-exploring-consumer-attitudes-to-iot/) of how personally identifiable data is being used, the regulations around data security are likely to get more strict, not disappear.

  

In healthcare’s Web3, it is crucial to balance data security regulations without crushing potential innovation.

  

An infrastructure that is compliant with existing and increasing regulations on data security, but also fosters innovation and decentralization can create the balance needed for healthcare’s future in Web3.

  

This infrastructure is Nectar.



# Introducing: Nectar



Nectar is a publicly accessible, highly scalable, privacy preserving, regulatory compliant network that creates a data rich environment for Web3 in healthcare. 

Nectar is an open source protocol built using multi-round interactive, optimistic rollup technology and is secured by the Ethereum blockchain. Rollups take processing off the main chain (Layer 1) by computing, storing, and batching transactions off-chain (on Layer 2). This creates a dramatic 100x scaling effect compared to L1, enabling up to 4,500 transactions per second. Rollups paired with Ethereum’s future Eth2 sharding increases throughput beyond 100,000 transactions per second. This high throughput is required in order to meet the existing demand of 82 million daily healthcare transactions globally.

Rollups that use multi-round interactive fraud proofs secure the transaction at the lowest Layer 1 (L1) gas cost possible. This is thanks to a special protocol that, when a final transaction is challenged as potentially fraudulent, the protocol “dissects” the assertion to the lowest level possible to identify whether the initial or challenger assertion is correct. This dissection occurs off-chain, and the final result is put on-chain as a much smaller transaction than if the entire dissection was on-chain, or if re-execution was used (which re-executes the transaction on-chain). Given the potential complexity and size of enterprise level and healthcare-specific smart contracts, a protocol that conducts its fraud proof off-chain reduces the L1 gas cost to as low as possible is ideal. In addition, keeping the challenge process off-chain and submitting the final transaction with a zk-Proof is one way in which the rollup architecture preserves data privacy.

Despite enterprises' history of experimenting on private blockchains, Nectar is intentionally secured by Ethereum. Public blockchains, such as Ethereum, provide stronger security, immutability, transparency, lower costs, and the ability to interoperate with other applications compared to private blockchains. Rollups can offer the privacy and security required for enterprise, while offering the additional benefit of public blockchains. 

In order for healthcare enterprises to reap the benefits of a public blockchain, the technology must be safe to use and regulatory compliant, which means adhering to existing data privacy and security regulations. In addition to keeping transactions off L1, Nectar accomplishes regulatory compliance in two additional ways:


Pre-Authorized Nodes
Privacy Preserving Contracts

The nodes in Nectar are called Data Service Providers (DSPs) and they are required to adhere to HIPAA guidelines by running HIPAA compliant servers and maintaining certain policies for the safe storage and transfer of healthcare data. HIPAA was chosen as the first regulatory requirement in Nectar because it is the most well known, widely used healthcare data security regulation, and it is not overly onerous to implement compared to other regulations such as GDPR. (Nectar is not limited to just HIPAA compliance.)

Adherence to HIPAA is initially assessed in a pre-authorization process prior to a DSP joining Nectar. To maintain compliance, DSPs participate in regular audits of HIPAA compliance; passed audits enable DSPs to remain in the network; failed audits kick DSPs out of the network. 

Nectar also offers a Bring Your Own Node option where the user or dApp developer can run their own HIPAA compliant node in order to keep their data fully private and to adhere to regulatory requirements for data accountability even if it is.

The privacy-preserving nature of Nectar comes from Permissioned Smart Contracts and Private Smart Contract Invocation. The focus on privacy preservation is what makes Nectar accessible to the behemoth enterprises that are leading Web3 innovation. It can encapsulate smart contacts, restricting access to only those authorized.

By creating a highly-scalable yet private and low-cost blockchain environment, enterprises can confidently use this technology to drive Web3 innovation.

HIPAA compliant DSPs also create the distributed data storage infrastructure of Nectar. Private data analytics is a promising, efficient Web3 technology and can have a significant impact on cost savings for enterprises. While individuals and small businesses are likely to adopt distributed data storage before enterprise, the potential for better security, lower cost, and new revenue streams for enterprises will be more enticing than simply shifting an on-prem server to a cloud-based provider.

Nectar’s unique combination of roll up technology, focus on privacy preservation, and HIPAA compliance creates the needed foundation for the Web3 future of healthcare. 

# Nectar Rollup Deep Dive

  

The Nectar Protocol is based on Arbitrum’s Open Source Code with certain modifications to ensure healthcare compliance. This document assumes that you will access [their exceptional documentation](https://developer.offchainlabs.com/docs/inside_arbitrum#fees) for Arbitrum-specific detailed technical specifications.

## Why Rollups

  

The purpose of Nectar is to enable the future of healthcare through novel technologies and incentive alignment. Web3, specifically with a blockchain foundation, is this future.

  

However, blockchains, in their current form, have flaws that prevent its leading role in the future of healthcare:

  

1.  Limitation in transaction throughput
    
2.  Expensive transaction costs
    
3.  Public transactions for complex computations
    

  
  

These don’t work for healthcare, and especially as a foundation for driving innovation in healthcare because:  
  
  

1.  82 million transactions occur daily in healthcare globally
    
2.  Spending on healthcare (3.9%) is [growing faster](https://www.who.int/health_financing/documents/health-expenditure-report-2019.pdf?ua=1) than the global economy (3.0%)
    
3.  Identifiable healthcare data has strict privacy regulations, and generally, data privacy laws are becoming more strict
    

  

When considering options that work for healthcare’s Web3 blockchain infrastructure, Layer 2 technology ticks all the boxes:

  

Layer 2 works for healthcare because it enables a compliant infrastructure that has abundant and accessible open source code, transactions are faster and cheaper than Layer 1, and certain implementations can offer total privacy with the benefit of being secured by a Layer 1 chain.

  

There are many Layer 2 options to choose from: State Channels, Plasma, Side Chains, and Rollups. But only the last 2 make sense for healthcare.

  

State Channels and Plasma are both restricted in their application, so they are not suitable for healthcare’s complexities, such as multi-party smart contract execution. And, Optimism [evolved](https://twitter.com/optimismPBC/status/1215410533052055553), leaving its plasma focus behind.

  

Side Chains and Rollups remain.

  

The Tamarin team has experience building Health Nexus, our healthcare-specific blockchain and is currently implementing consensus improvements via their ~$1M grant from the National Science Foundation.The Team’s experience in building a HIPAA-compliant protocol has transformed their understanding of the problems unique to healthcare. While Health Nexus may play a future role in bridging Nectar to other blockchains, the goal of creating a regulatory compliant way of using today’s public blockchains is possible using a Rollup where the data and transactions are handled privately off-chain.  
  

There are many reasons Rollup technology is ideal for Nectar:  
  

1.  Rollups increase throughput of any Layer 1
    
2.  Rollups cost less since contract execution occurs off-chain
    
3.  Rollups enable more use cases and more complexity than State Channels and Plasma
    
4.  Rollups offer scalable privacy preservation with and without the need for encapsulating the entire transaction in zero-knowledge technology
    
5.  Rollups inherit the security of the L1 consensus protocol
    
6.  Rollups remain advantageous after any Layer 1 scaling implementation
    

  

Some may argue that there are Layer 1 blockchains that already offer unmatched speed and low cost, such as Solana. We considered that, and also considered potential risks of betting on just one blockchain (i.e.: obsoletion).

  

This is another reason why rollups make the most sense: rollups can be blockchain agnostic, and can make any Layer 1 faster and cheaper.

  

### Optimistic vs. Zero-Knowledge? Both!

  

There are two types of rollups, optimistic and zero-knowledge. They differ technologically in their proofing mechanism, interactive vs. validity.

  

Both optimistic and zk-Rollups will eventually be available in Nectar. For now, Nectar is focusing on optimistic rollup implementation because zk-rollups are currently difficult and expensive to implement for complex transactions.



## Why an Arbitrum Base

  

We are not interested in re-creating the wheel, so open source code that is ready and developer friendly is important. There are currently two leading optimistic rollup solutions: Optimism and Arbitrum.

We landed on Arbitrum over Optimism because Arbitrum uses multi-round interactive proofs which offer features required for a healthcare-focused technology:  
  

1.  *Limitless contract size and higher per-tx gas limit*: In the case of a dispute, large transactions may require many interactive steps to get to the final step. But, because only the final dispute step is posted to L1 contract size and gas limits aren’t a concern. This is important because in healthcare, many processes are complex. It is easy to imagine large, complex contracts that support healthcare.
    

3.  *Implementation flexibility*: Healthcare is complex. The option for flexibility is important.
    

5.  *Lowest possible cost to secure on L1*: The purpose of interactive proving is to solve the dispute off the L1 chain and post just the resolution on the L1 chain. This is one step, compared to re-execution, which solves the dispute on the L1 chain, and creates the smallest possible L1 transaction, thus reducing a main cost-contributor to rollups.
    

  

In addition, [native tokens](https://developer.offchainlabs.com/docs/rollup_basics#cross-contract-communication) can be minted on rollup chain. Nectar has a long-term plan of becoming a global network for healthcare and Layer 1 agnostic. Native tokens would enable utility; unique healthcare tools and services that are not restricted by geographical boundaries; and the ability to create a data web and data asset future.

  

Arbitrum has created a dispute resolution protocol that is privacy-preserving, which is the perfect foundation for the private smart contract system needed for healthcare applications. While there are modifications necessary to Arbitrum in order to be more functional for healthcare, Arbitrum has solved key issues with L1 and L2 technology that create a perfect foundation for Nectar.

  

## Arbitrum Optimistic Rollup Architecture

  

Before we dive into the modifications, we’ll cover the key components of Arbitrum’s optimistic rollup architecture. (Reminder that this document assumes that you will access [their exceptional documentation](https://developer.offchainlabs.com/docs/inside_arbitrum#fees) for the minute details of the technology.)

  

![](https://lh4.googleusercontent.com/D24WK9dE_83F7QgR6TwOBCYxDSS0dhS7Coh5RgzYhFg14pCNnm7qzpx50eIc_YBafkbvxEalULntOOacfBLrXvGUhuBfdHNoS-kDZlKVa1UxaLSe9aJLSHD5nz2PSGdlkIrgsSsY=s0)

Source: Arbitrum [Website](https://developer.offchainlabs.com/docs/inside_arbitrum)

  

Arbitrum’s Rollup Architecture includes the following components:

  

-   Arbitrum Chain: the rollup chain and its contents, listed below
    
-   ETHbridge: Ethereum-based contracts that are the ultimate authority of what’s going on in the Arbitrum Chain by tracking the inbox, chain state, and outbox.
    
-   Rollup Protocol: Composed of the Rollup Contract and Challenge Contract and within the Ethbridge; manages the multi-round interactive proving process of the rollup
    
-   AVM Architecture: Provided by Ethbridge; the interface between L1 and L2; L2 runs on the AVM; every Arbitrum Chain has its own AVM
    
-   ArbOS: the workhorse of the Arbitrum System; Computation, storage, and management of fee collection occurs in ArbOS
    
-   Validators: stakers for the multi-round interactive proving protocol
    
-   Full Nodes: the Full Node tracks the state of an Arbitrum Chain and provides an API so that others can interact with the Arbitrum Chain. Full Nodes can have optional roles such as:
    

1.  Aggregator: receives and batches transactions from users; an unlimited number of aggregators can exist
    
2.  Compressor: compresses transactions that are then uncompressed and read by ArbOS; helps save on L1 call data space
    
3.  Sequencer: an entity that is given authority to order transactions in the inbox of an Arbitrum Chain with the intention to provide finality instantly
    

  

## Modifications to Arbitrum

To cover modifications, we’ll start at the “top” and move toward the Ethereum chain (opposite to how we introduced Arbitrum’s features where we started with the Ethbridge and moved “out” to Full Nodes).

  

A reminder that a key issue in healthcare is regulation around how protected health information is handled (PHI). PHI has information or details in the data that could be used to identify an individual. For example, the United States has [18 identifiers](https://cphs.berkeley.edu/hipaa/hipaa18.html) which include data points such as name, age, zip code, and even diagnosis or procedure. However, using de-identified data is not possible for the millions of healthcare providers across the globe, and the millions of daily healthcare transactions. The identity in certain data is required for obvious reasons.

  

Additionally, smart contracts can contain potentially anything - including PHI. It may be hard to imagine why PHI would be needed in a smart contract, but it was also hard to imagine AirBnB or Lyft when the internet started.

  

Creating an environment where folks can responsibly use PHI in decentralized technology enables the utmost flexibility in finding ways to fix healthcare. As healthcare (and other industries) become more digitized, regulations are certain to change. But, change will be gradual over time. Regulatory compliant infrastructure has survivability and is best suited to positively influence innovation that will fix healthcare.

  

While the goal of Nectar is to support healthcare globally, Nectar will first start with ensuring HIPAA compliance since HIPAA covers healthcare in the United States and, well, since the US has [lower utilization but higher cost](https://www.commonwealthfund.org/publications/issue-briefs/2020/jan/us-health-care-global-perspective-2019), ranks [dead last](https://www.commonwealthfund.org/publications/fund-reports/2021/aug/mirror-mirror-2021-reflecting-poorly) in access to care, administrative efficiency, equity, and health care outcomes among other high income countries in the world -- there’s a lot of fixing needed. HIPAA also covers healthcare providers, so by focusing on HIPAA first, it ensures that tools built on Nectar can include tools geared towards healthcare providers and facilities. Not including providers and facilities would greatly narrow how Nectar could increase access to and decrease the cost of healthcare. Lastly, HIPAA is a good foundation for broader data privacy policies such as State-based data privacy laws in the United States or high-impact data privacy laws such as GDPR, which is consumer centric and is applicable to other countries that EU residents travel to.

### Data Service Providers = Nodes

  

In Nectar the biggest difference is that Data Service Providers power the Network and provide HIPAA compliance.

  

Data Service Providers (DSPs) can be individuals or businesses and can serve as Full Nodes, Validators and - roles unique to Nectar - as Authorizers, Auditors, Decentralized Data Providers. Full Node and Validator roles are covered here. Decentralized Data Services are covered here.

  

DSP Authorizers and DSP Auditors monitor HIPAA compliance for the Network. In the testnet launch of the Network, DSP Authorizers and DSP Auditors will be approved by Nectar representatives. For the mainnet, Nectar will transition to a decentralized approval process of DSP Authorizers and DSP Auditors, mirroring Proof of Authority models.

  

DSP Authorizers assess HIPAA compliance of DSPs and manage the first step for DSPs to join Nectar. DSPs are identifiable and are assessed for HIPAA compliance which includes written policies, training, and data security practices. Nectar will publish HIPAA requirements publicly so any individual or entity has the opportunity to apply as a DSP.

  

The second and last step for DSPs to join Nectar is via a HIPAA audit by a HIPAA Auditor. The DSP can request DSP Auditor services any time after being approved by a DSP Authorizer. The HIPAA Audit confirms that HIPAA compliance has been implemented appropriately. If the audit is passed, the DSP can join the network. If the audit is not passed, the DSP can choose to implement needed changes or not participate in the network. DSP Auditors conduct audits quarterly as required by HIPAA.

  

A key aspect of HIPAA compliance is executing and maintaining [Business Associate Agreements](https://www.hhs.gov/hipaa/for-professionals/covered-entities/index.html). Business Associate Agreements (BAAs) are mandatory agreements between a Covered Entity and a Business Associate (BA). See the section on Healthcare Data Compliance for more details.

  

Additionally, if a Business Associate (BA) works with a contractor, and that contractor has access to the BA’s PHI, then the contractor and BA must co-sign a Business Associate Subcontractor Agreement. This ensures that both the BA and Subcontractor are aware of and take steps to ensure the security and safety of the PHI.

  

When DSPs join Nectar, they automatically sign Business Associate and Business Associate Subcontractor Agreements. This process is managed by a smart contract.

  

When DSPs are approved, the HIPAA Auditor will categorize the DSP as a: Covered Entity, Business Associate, or Contractor (i.e.: neither a Covered Entity nor Business Associate, which means the DSP can fulfil the Contractor role) which will trigger the correct BAA for execution. However, BAAs, not BASs, will be required for all DSPs in the same chain when there exists one Covered Entity (CE). This is because of the composability within the chain, and the BA role with a CE.

  

While generally BAAs and BASs have standard content, some parts of the agreement are variable, such as the amount of insurance coverage based on the amount of data under management, and some Covered Entities are strict about the contents of their agreements.

#### Incentivizing HIPAA Compliance

  

In order to ensure proper compliance by DSPs, DSP Authorizers, and DSP Auditors, Nectar has certain controls in place. First, a DSP Authorizer and DSP Auditor cannot be the same individual or entity. The individual or entity can serve as a DSP Authorizer or DSP Auditor, but cannot be both at the same time. This is to prevent a DSP Auditor from auditing a DSP that it had just authorized in a DSP Authorizer role. A DSP Authorizer or DSP Auditor can change its role annually.

  

Second, Nectar has built-in incentives via risk sharing to ensure proper compliance by DSPs, DSP Authorizers, and DSP Auditors. HIPAA breaches are required, per federal law, to be reported and can result in a financial penalty to the DSP. To incentivize and support compliance within the Network, the DSP, DSP Authorizer, and DSP Auditor are in a risk-based arrangement. This means that they share in the upside (revenue) and downside (penalty). The percent of risk sharing is dependent on the role. For example, upside and downside risk is higher for the DSP because the DSP manages the data day to day. The percent of risk sharing is higher for the DSP Auditor than the DSP Authorizer because the DSP Auditor interacts more with the DSP via the initial and quarterly audits. In future versions of Nectar, we aim to allow DSPs, DSP Authorizers, and DSP Auditors to adjust their risk sharing percentage allowing more flexibility and creativity. For example, a DSP Auditor could charge lower up-front fees for a higher percent of upside and downside risk sharing. This risk-based arrangement also opens the opportunity for a decentralized insurance model within Nectar.

  

## Technical Modifications

  

*Pre-authorized Nodes*

The validator network consists of HIPAA-compliant DSPs which are contractually obligated to handle data in accordance with security rules as stipulated by federal regulations. These DSPs are legal entities that have executed BAA agreements on chain, allowing us to associate specific blockchain accounts to these legal entities. To facilitate our privacy-preserving compliant network, modifications need to be made that prevent unauthorized nodes fulfilling the role of a DSPs. Network traffic between DSPs and from the Nectar client will only be permitted between approved entities.  
  

*Governance*

The Nectar network relies on authorized DSPs requiring on-chain governance to maintain the network. Modifications to the Nectar client and on-chain contracts are required to facilitate this governance. See the governance related portions of these documents for more details behind the structure proposed.

  

*Privacy-Preserving Smart Contracts*

To enable privacy preserving contracts some changes to the way transactions are called, smart contracts are accessed, and data is made available are required.  
  
*Permissions for Smart Contracts*

To regulate access to data contained in smart contracts we are adding permissions such that contracts can be made private, with access only permitted for pre-specified accounts. Before a user can access a smart contract they will have to prove they are authorized to do so. This change means that composability between contracts can be restricted as needed. It also means that the global state of Nectar's smart contracts are private, and discreetly revealed as needed, for those authorized to see it.

  

*Private Smart Contract Invocation*

To invoke a smart contract, a signed request is made to access the contract (and any composed contracts). Once authorized, a user is free to interact with the contract. A transaction is created locally, and submitted securely to the DSP network. A transaction receipt along with the hash of the pre and post contract state is sent to the aggregator to include in a batch. On Nectar the aggregator is a public function that can be done by anyone, since an aggregator can always create a batch from a single transaction, Nectar inherits the same censorship resistance as Ethereum.  
  
After aggregating and sequencing the transaction is processed by the DSPs, and a result is created for inclusion into the next rollup block.  
  

*Zero Knowledge Proof verification*

The fraud proof mechanism described in Arbitrums protocol is a multi-round interactive resolution process where only the final dispute step is made public. This step has the potential to share potentially private information, as the step describes a single state change inside an smart contract. Because of the risk of exposing private information, the final resolution step needs to be encoded into a zero knowledge proof to prevent possible leaking.  
  
Using Arbitrums dispute resolution to reduce a complex set of state changes down to a singular state change we can express the proof in binary terms such that existing zero knowledge proofs can be efficiently employed. This combined with private transaction invocation enables the preservation of private data inside smart contracts.

  

*Extensible Rollup Blocks*

In order to provide future networks of DSPs that selectively offer varying decentralized services, Nectars roll-up blocks belong to a unique network that defines the type of services and the state hashes of the resources those services provide. Two networks are planned at the start, a decentralized storage network that secures files in regulatory compliant data stores, and compliant smart-contract services. As future technology emerges new data services will be able to create a unique chain of Nectar blocks for those services.  
  
*Decentralized Data Storage Service*

The previous modifications were aimed at securing smart contracts state and execution. With this change we’re extending the ability of smart contracts to interact with external decentralized data. This is accomplished by creating a seperate network of authorized DSP nodes that manage decentralized data storage. DSPs provide data storage using regulatory compliant data storage, and securing access to the data by deploying a data handling contract on the smart contract network. These DSP-deployed data storage contracts contain relevant meta-data and permissions as well as methods for accessing the data and meta-data.

  

Smart contracts with permission to interact with the data-storage contract will be able to access the meta-data and reason about the properties of the data including: type, availability, and access.

  

Data access is provided through interacting with the data-storage contract. The system is designed such that different types of data may have their own data-storage contract that provide additional interface options.



## About The Team



  

Nectar is being developed by the team behind Tamarin Health. Tamarin is backed by Boost VC, which is led by Adam Draper, and has received over $1 million in grants from the National Science Foundation for their blockchain in healthcare work.

  

Nectar is the next project by the Tamarin team. While our Nectar GitHub is currently empty, except for our documentation paper!, our experience of healthcare and blockchain started in 2016, and Nectar is the culmination of our experience. It is simply the next logical step to bring healthcare into Web3, and we’re kicking it off with this grant.

  

As Adam Draper said about healthcare and blockchain: "It is a massive opportunity, but the [folks] going after it will have to have a lot of experience in healthcare. The thing we have learned about healthcare is that it's sort of a club, and you can't get in unless youre already in. Its fascinating."

Three of Nectar's 4 team members have healthcare-specific graduate degrees; 2 of the 4 have worked in healthcare and healthcare administration, one at Yale New Haven Health System and has over 10 years of experience working in healthcare; and 2 of the 4 are blockchain engineers.

The team behind Nectar comes from both healthcare and blockchain.

Healthcare is broken and complex. But it is fixable, and the opportunity for innovation is limitless.

The future of healthcare is built on Nectar.

# Other Stuff

  

## On Healthcare Data Compliance

  

By 2025, global data creation is expected to reach [163 zetabytes](https://www.import.io/wp-content/uploads/2017/04/Seagate-WP-DataAge2025-March-2017.pdf) - a trillion gigabytes.

  

In anticipation of this and the growing power of dominant tech company’s access to and utilization of individual’s data, it’s no wonder that regulations around data security and privacy are increasing, globally: the General Data Protection Regulation (GDPR) in the European Union was passed in 2016; the California Consumer Privacy Act was passed in 2018; and China’s data protection law passed in [2021](https://www.reuters.com/world/china/china-passes-new-personal-data-privacy-law-take-effect-nov-1-2021-08-20/), just to cite a few examples.

  

More regulated industries such as healthcare, in contrast, have had strict data security and privacy laws in place for much longer.

  

The most well-known and globally implemented example of healthcare data security and privacy laws is the United States Health Insurance Portability and Accountability Act ([HIPAA](https://www.congress.gov/104/plaws/publ191/PLAW-104publ191.pdf)) of 1996

  

(Note: Hipaaaaaaaaaah. It’s HIPAA. There is no relation to, or protection for, Hippos 🦛 )

  

Many folks know the surface level intent of HIPAA: it protects data that can be traced to an individual. Stated differently, it protects personally identifiable health information.

  

Specifically, it requires:

-   written policies (policies and contractual agreements)
    
-   behavioral expectations (human behavior); and
    
-   technological security (data movement and storage)
    

  

These requirements are specifically for [Covered Entities and Business Associates](https://www.hhs.gov/hipaa/for-professionals/covered-entities/index.html).

  

Covered entities are:

-   Healthcare providers (such as doctors, nurses, chiropractors, or pharmacies)
    
-   Health Plans (i.e.: insurance companies, health management organizations, employer health plans)
    
-   Healthcare data clearinghouses (i.e.: companies that collect and sort data and then make millions of dollars selling your de-identified data)
    

  

Business Associates are businesses that receive, process, analyze, store, use, etc. data from Covered Entities (doctors, insurance companies, etc.) listed above.

  

And, if Business Associates work with other companies, those companies are also required, via contractual agreement, to adhere to strict protocols for data security and privacy. This creates a chain of contractual agreements that link back to the Covered Entity.

  

Failure to comply results in hefty fines and a listing on the HIPAA [Wall of Shame](https://ocrportal.hhs.gov/ocr/breach/breach_report.jsf) 😃

  

While it is true that healthcare data policies are due for an upgrade, specifically [in the United States](https://www.reliasmedia.com/articles/140405-big-data-in-healthcare-privacy-is-major-ethical-concern), the regulations are not likely to go anywhere (especially in light of growing data regulations for non-healthcare data).

  

Thus, in order to drive innovation and to build the data web that underpins the future of healthcare, the access, storage, and transportation of personally identifiable health data must be regulatory compliant.

  

The reader with a keen eye will think, “but what if the patient owns their data or the data doesn’t originate from a Covered Entity at all?” as a way to escape data regulation.

  

This is a great point. It is correct that if the data does not originate from a Covered Entity then HIPAA rules do not apply.

  

However, excluding personally identifiable data from the best and original source: the patient visit, creates a weak dataset. Wearable data, in and of itself, is not that [helpful](https://mhealth.jmir.org/2021/3/e20738); and it would take an incalculable amount of time to manually (yes, manual. Most physician offices still send your data by CD) collect data via only the patient-directed route.

  

The best data set combines data that would fall under HIPAA and patient-provided data (such as data that has been reviewed and approved by the patient; wearable data).

  

It is crucial for decentralized and Web 3 technology to adhere to healthcare data regulations.

  

Regulatory compliance aside, there’s a growing concern for how health information is being or could be used, and an expectation that data remains safe, even if it didn’t originate from a Covered Entity. Concern of data privacy was one of the cited reasons many rejected vaccination passports during the COVID-19 pandemic (which is actually an incorrect interpretation of HIPAA). And, there is substantial concern among clinicians, professionals, and patients with the large tech firms (GAFA) gaining access to healthcare data for [their own profit](https://www.bbc.com/news/business-57817804).

  

So even if HIPAA doesn’t legally apply, many want their healthcare data protected and safe.

  

When folks express anger toward the healthcare industry, the anger isn’t that they don’t want their data to be secure and protected. The anger is toward how the healthcare system runs. It’s:

  

-   The asynchronous nature of care and data accessibility
    
-   The general inability to access data due to greedy business practices
    
-   Misaligned incentives
    
-   The reimbursement model that rewards sick care (payment based on number of procedures) instead of based on well-care (payment based on healthy outcomes)
    
-   The infuriating cyclical process of prior-authorization required before care can even be provided
    
-   The resulting administrative hours wasted to get insurance coverage of the procedure
    
-   The cost, inefficiency, and time (spanning years, sometimes decades) of the clinical trial process required to get to the regulatory approval process for devices, medications, or therapies
    
-   The length of time it takes for regulatory approval of devices, medications, or therapies including novel therapies such as psychedelic therapy
    
-   The inefficiency of the supply chain process, and ease of disruption to the supply chain process akin to 2020 delays during the COVID-19 pandemic
    
-   The technologically outdated processes for training and re-licensure
    
-   The lost time and compromise to patient care caused by credentialing delays
    

  

This is why Nectar exists. Nectar complies with data security regulations so that innovation is not shut down.

  

HIPAA compliant nodes add extra protection for patients in countries with less-strict or non-existent healthcare data privacy and security regulations. And, for countries with more strict regulations than HIPAA, HIPAA serves as a base for compliance. Nodes in Nectar can differentiate themselves by implementing other healthcare data privacy and security regulations to follow.

  

​​We chose to start with HIPAA because it is the most widely known and used healthcare-specific data protection regulation, and it is also not overly onerous to implement. It’s a good starting point. Nectar will add other regulatory requirements to make the network extensible outside healthcare, such as GDPR or state-based data privacy laws such as those in California, Virginia, and Colorado.

  

Nectar is compatible with any other data security and privacy regulations. Nodes can offer and market their additional data privacy and security services that help application developers remain compliant with other regulations such as the United States Family Educational Rights and Privacy Act (FERPA) of 1974; Gramm Leach Bliley Act (GLBA) for banks in the United States; Virginia's, California’s, and Colorado’s data privacy acts (a growing trend in the United States); or GDPR which covers all of the European Union. As data grows, so do the requirements for protecting that data.
