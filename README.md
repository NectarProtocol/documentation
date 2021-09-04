# Nectar Protocol


## Introduction



  
In 2014, the [Living Heart Project](https://www.3ds.com/products-services/simulia/solutions/life-sciences-healthcare/the-living-heart-project/) kicked off, debuting the first simulated real-life heart. Powered by the 3DExperience platform from Dassault Systèmes, the research has brought together leading physicians, researchers, educators, medical device developers, regulatory agencies, and practicing cardiologists from across the world to develop personalized digital heart models. The project just received additional federal funding, expanding the scope to virtual patients and computational modeling.

  

In 2017, an article in The Journal of Arthroplasty found that [personalized knee replacement](https://www.arthroplastytoday.org/article/S2352-3441(17)30040-7/fulltext) devices had far better outcomes at no additional cost than “out of the box” knee replacement devices.

  

In 2018, a [study](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6202760/) was published in Acta Orthopaedica about a December 2017 shoulder replacement surgery on an 80-year old woman with advanced arthritis. This surgery was guided by Microsoft’s HoloLens, which personalized guided steps for the surgery based on the patient’s medical history and operating technique which were accessible and visible in real time via the HoloLens: “the surgeon was able to compare, stage by stage, what he was doing with what had to be done” for the surgery.

  

In 2019, a surgeon in China successfully completed a liver removal of a lab animal over a 5G internet connection. The surgeon was at a different location [30 miles away](https://in.pcmag.com/news/128092/china-performs-first-5g-remote-surgery).

  

In 2020, because of the COVID-19 Pandemic, clinicians in the United States were allowed to practice telemedicine [across state borders](https://www.hhs.gov/coronavirus/telehealth/index.html) without concern to their State Licensure. In 2021, the Center for Care Innovations presented a host of evidence that, for many clinical applications, telemedicine was [*just as, if not more effective*,](https://www.careinnovations.org/virtualcare/resources/evidence-for-telemedicine-efficacy-and-quality/) than in-person care.

  

In 2021, the opportunity of *in silico* trials (trials performed by computer simulation) promises [better, faster, and cheaper clinical trials](https://trialsjournal.biomedcentral.com/articles/10.1186/s13063-020-05002-w).

  

The future of healthcare is exciting. The future of healthcare is Web3.

  

The future of healthcare is not bound by geographical boundaries; it blurs the line between reality and digital; it is more effective and less expensive; it is data rich.

  

But, healthcare has strict data and security protocols and regulations - specifically for personally identifiable data.

  

The key to Web3 for healthcare is *personalized medicine* which is made possible by *personalized, identifiable data*.

  

But, “ethical issues related to fair and responsible data usage, as well as privacy, ownership, security, and authentication are paramount.”

  

Cutting edge, Web3 innovation cannot ignore data and security protocols and regulations, no matter how outdated the regulations are.

  

Additionally, innovation occurs at the enterprise level.

  

-   The Living Heart Project was initiated by Dassault Systèmes, a company founded in 1981 with €4.5B annual revenues;
    
-   The personalized knee replacements were conducted at a teaching hospital;
    
-   The HoloLens shoulder replacement was conducted at a 1,097 bed hospital in France (to compare, Massachusetts General, one of the leading hospitals in the United States, has 1,059 beds - these are large teaching institutions)
    
-   The remote surgery in China was conducted by a surgeon from Beijing's 301 Hospital which has 4,000 beds
    
-   While telehealth was started by startups, the leading telehealth company is now valued north of $15B (and they've been HIPAA compliant since they began)
    
-   And, *in silico* trials are led by researchers which are either in teaching and university institutions or, if a startup, came from teaching and university institutions
    

Enterprises do not skimp on data and security practices.

  

We’ve also learned, from Web1 through Web2, that public networks (Internet vs. Intranet) and [open source software](https://ieeexplore.ieee.org/document/7160503) are leading factors in innovation.

  

The future of healthcare requires a foundation that fosters innovation in an open, accessible, data rich, regulatory compliant way, while remaining flexible enough to accommodate data and security policies that inevitably modernize.


The future of healthcare is built on Nectar.


Introducing: Nectar
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



## About The Team



  

Nectar is being developed by the team behind Tamarin Health. Tamarin is backed by Boost VC, which is led by Adam Draper, and has received over $1 million in grants from the National Science Foundation for their blockchain in healthcare work.

  

Nectar is the next project by the Tamarin team. While our Nectar GitHub is currently empty, except for our documentation paper!, our experience of healthcare and blockchain started in 2016, and Nectar is the culmination of our experience. It is simply the next logical step to bring healthcare into Web3, and we’re kicking it off with this grant.

  

As Adam Draper said about healthcare and blockchain: "It is a massive opportunity, but the [folks] going after it will have to have a lot of experience in healthcare. The thing we have learned about healthcare is that it's sort of a club, and you can't get in unless youre already in. Its fascinating."

Three of Nectar's 4 team members have healthcare-specific graduate degrees; 2 of the 4 have worked in healthcare and healthcare administration, one at Yale New Haven Health System and has over 10 years of experience working in healthcare; and 2 of the 4 are blockchain engineers.

The team behind Nectar comes from both healthcare and blockchain.

Healthcare is broken and complex. But it is fixable, and the opportunity for innovation is limitless.

The future of healthcare is built on Nectar.
