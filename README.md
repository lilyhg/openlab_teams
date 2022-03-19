# openlab teams
OR "Open Source, Open Science and the laboratory of the future"

## Specification
a simple GUI tool to:
 * create metamask, multisig wallet on polygon and set up coordinape
 * prompt to set up a GitHub repository with manubot already pre-loaded and a solid directory template
 * prompt to set up a Slack/Discord with Github and Coordinpape integration
 * tool to "publish" github repository by minting an NFT
   * export GitHub repository snapshot to IPFS with intact directory structure. Cover image of the NFT can be a visual abstract of the work.
   * enable threshold encryption of GitHub export using LitProtocol and mint access-controlling NFT (if desired)
   * perform fractionalization of the NFT
   * distribute the fractionalized NFT according to the balance of $GIVE tokens on coordinape

## Problem
The web has enabled the rapid development of open source software. By bringing together contributors from around the globe with intrinsic motivation and the right talent to contribute to a project, open source communities are able to produce work that is on par with comparable closed source projects developed within for-profit entities. 

Open science takes inspiration from the open source movement and aims to apply it to the process of scientific research. While an increasing number of academic researchers support the goals of the open science movement, the funding, execution, and distribution of scientific projects are still very centralized. For example, the NIH is the largest funder of academic research in the US by far, experiments are mostly executed in the laboratory of the PI that won the grant, and results are published in a legacy system with the PI's intellectual property being partially controlled by the host institution.

Why has open source been such an overall success, while open science is still lacking behind? We believe the difference between open source code and open source science is the transaction cost of sharing work. While code has a low cost of execution and high reproducibility, the opposite is true for most scientific work. Both laboratory services and more complex machine learning models often come with high upfront costs to repurpose them. A possible solution to reducing the upfront cost of setting up a laboratory or computational process is a peer-to-peer exchange on which scientists can offer services to each other. We believe an open exchange of laboratory services, akin to a global network of small and large core facilities, will begin a new epoch of scientific laboratories. The academic laboratory of the future will be a slack/discord server with a GitHub repository. The laboratory members will be a global group of scientists and students united by tokenized ownership of their work.

## Solution
An open exchange of laboratory services will allow other scientists to book a service from a peer to be applied to their own scientific question in return for shared ownership of the result and/or money. This will enable scientists to explore alternative sources of research funding, lead to sustainable maintenance of useful scientific tools, and will drive standardization of experimental procedures. In the long run, we envision that the open transaction data coming from such an exchange will contribute to a global scientific knowledge graph and alternative metrics for scientific excellence.

The key invention enabling such an exchange to exist are web3 open source payment systems, also referred to as cryptocurrencies, and decentralized data management, often used for applications like NFTs. While an open peer-to-peer exchange for laboratory services could -in theory- be built without such web3 applications, the amount of legal engineering required to enable permissionless and international peer-to-peer payments, intellectual property management and collaboration approaches the impossible.

At LabDAO we are developing the openlab exchange, a set of smart contracts, APIs, and plugins that enable scientists to share their developed tools with peers. We begin with decentralized bioinformatics compute and data storage. Scientists uploads their data to an open, community-run IPFS storage system using our command-line interface. They then submit a job, for example, an RNA-Seq nextflow-core run, and reference their uploaded data. After paying one of their peers running a server cluster with the specified application in tokens, the job is executed and the results are shared with the scientists using IPFS. While we are starting with bioinformatics, we are more ambitious than that. By the end of this decade, we want to see the first therapeutics on the market developed using dry and wet-lab tools made available via openlab.

Next to the exchange protocol, we are also working to define the basic organizational unit of this new era of scientific research. We call this project openlab teams. The scientific laboratories of the future will be online communities united by a shared scientific goal, a chat server, a GitHub repository, and a token that represents fractional ownership in the intellectual property that is generated over the course of the project. To facilitate the emergence of these decentralized organizations, openlab teams will help scientists launch their collaborative projects with a couple of mouse clicks.

## Technology
At the core of both the openlab exchange and openlab teams are decentralized storage protocols and tokens.

In the openlab exchange (previously named LAB protocol internally) users submit API requests using the openlab CLI to servers run by service providers. Within these API requests, users reference the input data using IPFS URIs. If access to the input data has to be controlled, threshold encryption can be used to mint a private NFT that grants access to the referenced data exclusively to the owner. After receiving the API request, the provider's server is checking that a payment deposit was made and that all required encryption keys to work with the data are available. If these criteria are met, the service provider gets to work and mints the results into new NFTs that are transferred in return for the user's payment. In case of conflict, market particpants can trigger an arbitration service to settle disagreements among the scientists.

The openlab teams product is enabling scientists to stand up their own scientific micro-organizations by minting all the data within a git repository on IPFS into a private or open NFT. This NFT is then subsequently fractionalized and can be given to lab members proportional to their contributions within the project. Co-ownership of scientific results will be the new co-authorship. Over time multiple of such project-based micro-organizations can be aggregated into larger organizations - very similar to how academic institutions contain multiple academic laboratories that in turn work on multiple scientific projects. In case financially relevant IP is generated within an organization, the owners of the fractional NFT tokens can sell their ownership using dedicated exchanges or launch their own for-profit entities.

Very little of what I have described above is already built. If you want to help us give science an overdue upgrade, get in touch via DMs or join our discord.
