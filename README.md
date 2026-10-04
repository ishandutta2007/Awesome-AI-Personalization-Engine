# Awesome-AI-Personalization-Engine

# Awesome AI Personalization Engine



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Real-Time Recommendations, Contextual Personalization & Reinforcement Learning*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Personalization Engines**. These tools help applications deliver relevant content, product recommendations, and experiences to each user based on behavior, context, and learned preferences.



**Examples** include Microsoft Personalizer AI, Dynamic Yield, Algolia Recommend, AWS Personalize, Bloomreach Engagement, Insider, Monetate, Coveo, Kibo Personalization, and Crossing Minds (the category leaders).



**Open-source emphasis**: The AI personalization engine space is **dominated by proprietary SaaS platforms**, but a **mature open-source ecosystem** exists for those who want full control over their recommendation infrastructure. **Gorse** (Apache-2.0) is the standout—a universal open-source recommender system written in Go with multi-source recommendations, LLM-powered capabilities, a GUI dashboard, and RESTful APIs . **LightFM** (Apache-2.0) provides hybrid matrix factorization for both implicit and explicit feedback with metadata support . **Implicit** (MIT) delivers fast collaborative filtering for implicit datasets with multi-threaded training . **Mr. DLib** offers recommendations-as-a-service for academic content . This section documents these production-grade solutions.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents



- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Microsoft Personalizer AI](https://learn.microsoft.com/en-us/azure/ai-services/personalizer/)**  

  **Reinforcement learning-based personalization service (retiring October 1, 2026).** Uses contextual bandits to select the best action for each user context, learning from reward feedback . **Key APIs**: **Rank API** returns the best action ID for a given context; **Reward API** provides feedback (0-1 score) to improve decision-making . **Learning modes**: **Apprentice mode** (learns from existing decision logic to mitigate cold start) and **Online mode** (explores and exploits) . **Retirement notice**: New resources could not be created since September 20, 2023; service retires October 1, 2026. **Migration path**: Microsoft recommends the open-source **microsoft/learning-loop** . **Use cases**: E-commerce product selection, content recommendation, ad placement, notification timing .



- **[Dynamic Yield](https://www.dynamicyield.com/)**  

  **Enterprise personalization and experimentation platform.** **Experience APIs** enable server-side personalization without client-side flicker, protecting internal strategies and user privacy . **Key APIs**: **Choose API** (primary endpoint for activating campaigns and returning variations); **Pageview API** (reports pageviews without campaign); **Engagement API** (tracks clicks and impressions); **Search API** (AI-powered semantic and visual search); **Event Reporting API** (Login, Add to Cart, Purchase, Video Play) . **Shopify Checkout integration** renders campaign content as native checkout UI components with selector names and targeting rules . **Deployment**: API-based for performance-sensitive campaigns, script-based for quick time-to-value, or hybrid .



- **[Algolia Recommend](https://www.algolia.com/doc/libraries/sdk/methods/recommend/get-recommendations)**  

  **AI-powered recommendations from the Algolia search platform.** **Related Products** model suggests items similar to the current product; **Frequently Bought Together** and **Trending Items** models available . **Threshold parameter** controls recommendation confidence. SDKs available for JavaScript, Python, Go, Java, C#, PHP, Kotlin, Swift, Dart . **Integration**: Works alongside Algolia Search for unified discovery and recommendation.



- **[AWS Personalize](https://aws.amazon.com/personalize/)**  

  **Fully managed ML service for real-time personalized recommendations.** Uses the same ML technology as Amazon.com with no ML expertise required . **Use cases**: Product recommendations, individualized search results, customized direct marketing, content carousels, ad placement . **Key features**: Real-time or batch recommendations; handles cold-start problems for new users and items; data encrypted and private; pay only for what you use . **Deployment**: API-based; integrates with websites, apps, SMS, and email .



- **[Bloomreach Engagement](https://www.bloomreach.com/)**  

  **AI-powered customer data platform and omnichannel marketing suite.** **Recommendations**: Uses collaborative-based models (ALS, word2vec) and **sequence-based models (two-tower neural networks)** to handle consecutive interactions and alleviate cold-start via metadata . **Predictions**: Decision trees, random forests, and gradient-boosted trees for purchase probability, email open, optimal send time, churn, and in-session behavior . **Scenarios**: No-code drag-and-drop journey orchestration with multi-agentic AI (Loomi AI) for automated scenario creation . **Training data**: User events including views, clicks, cart interactions, and purchases .



- **[Insider](https://insiderone.com/)**  

  **AI-powered personalization and customer experience platform.** **Key capabilities**: Turn anonymous traffic into customers without login; AI models predict intent for tailored recommendations and promotions; real-time personalization adapts banners, collections, and messaging . **Proven results**: Adidas 259% increase in AOV; MAC 17.2X ROI; Slazenger 49X ROI in 8 weeks . **Recognition**: 2025 Gartner Peer Insights Customers' Choice for Multichannel Marketing Hubs (4.9/5 rating); G2 #1 Leader across 11 categories including Personalization Software and CDP .



- **[Monetate](https://monetate.com/)**  

  **Enterprise experience optimization platform.** **Agentic AI**: Real-time adaptive intelligence that continuously learns, acts, and improves outcomes across personalization, recommendations, and experimentation . **Symphony & Maestro**: Symphony orchestrates AI, data, and decisioning into harmonized 1:1 experiences; Maestro delivers enterprise-grade experimentation without flicker . **Omnichannel**: Web, mobile, email, in-store, and customer care . **Developer-friendly**: Open APIs, SDKs, and CI/CD alignment . **Compliance**: HIPAA-ready, GDPR, CCPA, PCI-compliant .



- **[Coveo](https://www.coveo.com/)**  

  **AI-powered relevance platform for customer and employee experiences.** **Relevance Generative AI**: Synthesizes answers from unified content sources (Salesforce knowledge, community posts, PDFs, LMS modules, video transcripts) with citations . **Case Assist AI**: Classifies issues as users type, suggests categories, and generates answers to deflect cases . **Agent integration**: Rich context in CRM showing self-service journey before escalation . **Analytics**: Continuous learning from every search, click, and generated answer; knowledge gap detection and FAQ drafting .



- **[Kibo Personalization](https://docs.kibocommerce.com/)**  

  **Personalization and search platform for commerce.** **Product Suggest Settings** includes `personalizationExperience` parameter for configuring personalized product suggestions . **Search API** delivers personalized product discovery.



- **[Crossing Minds](https://www.mitacs.ca/our-projects/automatic-machine-learning-for-recommender-systems/)**  

  **ML-based recommendation systems with auto-machine learning research.** Companies integrate their data and obtain on-demand personalized recommendations . **Research focus**: Auto-ML for recommender systems to reduce customer onboarding turnaround time and improve scalability .



## Open-Source GitHub Projects



### Universal Recommender Systems



- **[Gorse](https://github.com/gorse-io/gorse)**  

  **The leading open-source recommender system engine.** **Apache-2.0 licensed**, written in Go . **Key features**: **Multi-source** — recommends from latest, user-to-user, item-to-item, collaborative filtering, and more; **Multimodal** — supports text, image, and video via embedding; **AI-powered** — classical recommenders and LLM-based recommenders; **GUI Dashboard** for pipeline editing, monitoring, and data management; **RESTful APIs** for data CRUD and recommendation requests . **Architecture**: Single-node training and distributed prediction; stores data in MySQL, MongoDB, Postgres, or ClickHouse with Redis caching; master node for training, worker nodes for offline recommendations, server nodes for online APIs . **Quick start**: `docker run -p 8088:8088 zhenghaoz/gorse-in-one --playground` . **Best for**: Teams wanting a complete, production-ready open-source recommender system with minimal setup.



### Collaborative Filtering Libraries



- **[LightFM](https://github.com/lyst/lightfm)**  

  **Hybrid matrix factorization for implicit and explicit feedback.** **Apache-2.0 licensed**, Python-based . **Key features**: **BPR and WARP ranking losses**; incorporates **both user and item metadata** into matrix factorization; represents users and items as sums of latent feature representations, enabling recommendations for new items and users . **Fast**: Multi-threaded model estimation . **Fork**: **rectools-lightfm** provides 10-15x faster inference than the original model . **Best for**: Teams wanting to incorporate metadata into collaborative filtering.



- **[Implicit](https://github.com/benfred/implicit)**  

  **Fast collaborative filtering for implicit datasets.** **MIT licensed**, Python-based . **Key algorithms**: **Alternating Least Squares (ALS)** as described in Collaborative Filtering for Implicit Feedback Datasets and Applications of the Conjugate Gradient Method for Implicit Feedback Collaborative Filtering; BPR and Item-Item Nearest Neighbour planned . **Multi-threaded training** using all available CPU cores; optional Intel MKL for faster linear algebra . **.NET port** available via NuGet . **Best for**: Teams wanting fast ALS-based recommendations on implicit feedback.



### Specialized Recommenders



- **[Mr. DLib](https://libguides.tcd.ie/libtech2019/mrdlib)**  

  **Recommendations-as-a-service for academic content.** Non-profit open-source project run by researchers at Trinity College Dublin and University of Konstanz . **Services**: Recommendations-as-a-service for academic products; academic outreach for content providers; real-world research environment . **Best for**: Digital libraries and academic platforms wanting related-article recommendations.



### Additional Strong Open-Source Options



- **Full Recommender Systems**: **Gorse** (Go, multi-source, LLM-powered, GUI) .

- **Collaborative Filtering**: **LightFM** (hybrid, metadata, BPR/WARP), **Implicit** (ALS, multi-threaded, fast) .

- **Academic**: **Mr. DLib** (recommendations-as-a-service) .

- **Note**: The open-source ecosystem lacks full-stack equivalents to **Dynamic Yield**, **Bloomreach**, or **Monetate** (omnichannel journey orchestration, experimentation, and CDP capabilities).



**Frameworks for building custom systems**: Combine **Gorse** for a complete recommender system with multi-source recommendations and GUI dashboard, **LightFM** for hybrid collaborative filtering with metadata, **Implicit** for fast ALS-based recommendations, and **Mr. DLib** for academic content recommendations. Add **PostgreSQL** or **ClickHouse** for persistence, **Redis** for caching, and **Docker** for deployment.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- AI personalization engines handle sensitive user behavior and preference data; ensure compliance with GDPR, CCPA, and applicable data protection regulations.

- **Open-source reality**: The open-source ecosystem for AI personalization is **mature at the recommendation engine layer** (**Gorse**, **LightFM**, **Implicit**) but **significantly behind commercial platforms at the orchestration and experimentation layer**. **Microsoft Personalizer is retiring October 1, 2026**—users should migrate to the open-source **microsoft/learning-loop** . **Gorse** is the standout open-source alternative, providing a complete recommender system with multi-source recommendations, LLM support, GUI dashboard, and RESTful APIs . However, **commercial platforms** (Dynamic Yield, Bloomreach, Insider, Monetate) provide **omnichannel journey orchestration, no-code campaign management, A/B experimentation, and CDP integration** that open-source alternatives require significant additional tooling to match. The open-source path is **genuinely viable** for teams wanting full control over their recommendation infrastructure and data.



---



**Made for data scientists, ML engineers, product personalization teams, and e-commerce technologists.**

Let's make AI personalization more open, transparent, and user-controlled.
