# 118. GPT-NL is bijna klaar, maar zoekt nu klanten én daadkracht van de overheid (2025-08-07) [link](https://www.youtube.com/watch?v=MEL4h29UF1g)


 # GPTNL Podcast Discussion

The podcast centers on GPTNL, a Dutch large language model under development by a team led by product manager Saskia Lensing. The discussion, held by hosts Daniel and Ben, explores how GPTNL is being built from scratch with legally compliant data, its design philosophy, use cases, technical workflows, and the broader impact on digital sovereignty in the Netherlands and Europe.

## Legally Compliant, Licensed Data

• GPTNL is developed entirely from legally verkregen (authorized) data. Instead of scraping the internet indiscriminately, the team actively asks permission from data owners and signs licenses with key players (for example, agreements with Dutch newsmedia associations such as DPG Media).  
• The revenue model reflects fair compensation: 50% of license revenue will be shared back with data providers. This approach contrasts with U.S. practices where data scraping may lead to legal gray areas and controversies.

## Technical Architecture and AI Workflows

• The model is designed as a large-scale language model with approximately 26 billion parameters—positioning it in a similar performance range as GPT-3/3.5—with a focus on strong Dutch language capabilities along with English support for governmental and commercial data.  
• Pretraining is carried out on a dedicated national supercomputer (“Snellus” by SURF) featuring 88 GPUs organized in about 22 clusters. The training phase is expected to run over several months (with the current plan involving two epochs and incremental fine-tuning releases).  
• After pretraining, GPTNL undergoes an instruction fine-tuning phase. The team generates a substantial set of question–answer pairs covering tasks like summarization, text simplification, and factual retrieval.  
• Reinforcement learning with human feedback plays a role in optimizing model responses. Instead of using traditional RLHF methods, they have adopted newer techniques such as Direct Preference Optimization (DPO) to speed up the model’s ability to learn preferred behaviors.

## Use Cases and Target Audiences

• Primary target customers include Dutch public sector organizations (like municipalities and the national government) that require reliable and locally accurate language processing for document summarization, email drafting, and extracting insights from large volumes of administrative texts.  
• Other potential sectors mentioned are telecom (optimizing call center conversations and customer contact analysis), healthcare, education, insurance, and banking.  
• The model is designed for professional use rather than as a consumer product, enabling high-quality summaries, simplification of complex texts, and customization for domain-specific tasks.

## Development Philosophy: Digital Sovereignty and Ethical Design

• A key motivation is preserving digital sovereignty by reducing dependency on American big tech alternatives. GPTNL is positioned as a compliant, Dutch alternative that integrates high-quality Dutch cultural and legal context—key for governmental and public trust.  
• Ethical considerations are built-in “by design.” The team has already integrated provisions to document data provenance, ensure privacy, and make the system compliant with European regulations (including upcoming AI Act requirements).  
• The discussion also touched on challenges such as handling gender-specific language in certain domains and balancing neutrality with context-specific customization. The model will allow further adaptation per customer group (for example, more conservative or progressive language use in specific sectors).

## Partnership Strategies and Ecosystem Development

• Instead of building a full end-to-end product (including frontends), GPTNL focuses on developing the core engine (the “model weights”). This enables market partners and integrators to build user interfaces and operational tools on top of the engine.  
• There are ongoing discussions with several European cloud providers and integration partners. The aim is to maintain operational independence by partnering with European alternatives rather than relying on U.S. cloud infrastructure.  
• The team’s collaboration extends beyond technical development. They have established a governance model that involves data providers (in a cooperative structure) so that investment, operational decisions, and revenue sharing are transparent and mutually beneficial.

## Funding, Timelines, and Future Rounds

• GPTNL was initially funded with €13.5 million, secured with appropriate business planning that accounted for compute costs (initially through renting clusters rather than outright purchase of expensive hardware).  
• The timeline aims for a first public launch around January of the following year, with successive releases and refinements over the coming months.  
• Further financing is anticipated; the team foresees that an additional €4–5 million could significantly boost the next iteration, with longer-term rounds potentially summing up to €10–15 million to expand capabilities.

## Broader AI Landscape and Comparison with Big Tech

• The podcast contrasts the Dutch approach with the American model. While U.S. companies sometimes push boundaries legally (e.g., Grok, with controversy about unauthorized data scraping), GPTNL emphasizes compliance and ethical data use.  
• Despite being smaller in scale compared to models from companies like OpenAI, GPTNL intends to differentiate itself by offering a tailored Dutch language solution with higher contextual and cultural accuracy.  
• There is acknowledgment that GPTNL will initially offer a subset of capabilities relative to best-in-class consumer models; however, the emphasis is on functionality for professional and governmental applications rather than all-purpose consumer usage.

## AI News and Future Outlook

• The conversation references recent U.S. launches and controversies (including mentions of Sam Altman, Elon Musk’s Grok, and shifting methods in reinforcement learning) as part of the broader AI news landscape.  
• Similar initiatives are appearing across Europe (e.g., in Sweden), but trust issues between model builders and data owners have surfaced. GPTNL aims to address those challenges through a transparent, consent-based, revenue-sharing approach.  
• The broader context points toward continuous investment in generative AI within Europe, with increasing demand from public and private sectors prompting further development of domestic, legally robust models.

Overall, the podcast provides an in-depth view of the technical, ethical, and commercial considerations behind GPTNL. The discussion reveals a deliberate path toward creating an AI that respects legal boundaries, integrates high-quality Dutch data, and positions itself as a cornerstone for both digital sovereignty and innovative professional applications in multiple sectors.