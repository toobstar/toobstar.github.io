+++
title = 'Emerging patterns of GenAI Governance and Risk Control'
date = 2025-04-02T13:04:53+11:00
draft = false
tags = ['Risk', 'CIO', 'AI', 'GenAI', 'AI Governance', 'Risk Management']
revision = 1
+++

![ChatGPT in rough waters](https://toobstar.github.io/images/pirate-ship-chatgpt.png)

In the rapidly evolving landscape of Generative AI (GenAI) organisations face the dual challenge of harnessing innovative capabilities to maintain competitiveness and advance their business while effectively managing the associated risks. 

I was interested to provide a concise overview of AI's progression and highlight the critical development of trust, governance and risk control measures in response to GenAI's widespread adoption. Key concerns such as data privacy, bias, and the correctness of AI-generated content are considered, alongside the emergence of ethical principles and governance frameworks aimed at mitigating these risks. The operational processes enabling GenAI also present many new cybersecurity risks which cannot be ignored. 

As businesses race forward into this brave new world, they must prioritise responsible and safe AI adoption to ensure long-term success.


## Generative AI: Slow, then fast, then *really* fast

Without providing a deep overview of AI the history and use of it is surprising long.  With early research and use happening alongside the establishment of computer science even from the 1950s and the likes of Alan Turing. The work back then focussed on rule-based systems and provided basic probabilistic models that could generate simple text.

Through the 1990s and early 2000s neural networks and deep learning approaches developed to provide more practical commercial applications, but it will still at the fringe of engineering practice.  It has been in the last 10 years that the tranformer revolution and Generative Adversarial Networks (GANs) enabled AI to create realistic images and videos that we saw the use of AI become more central to engineering R&D efforts.  The demonstrations of capabilities were so impressive they could not be ignored. 

And since 2020 with the widespread release of large scale language models (LLMs) based on the transformer architecture with the likes of GPT, DALL-E and Stable Diffusion we have seen the use of these become mainstream and the attention for all forward looking businesses to be focussed on GenAI as a potential approach to rapidly improve product and service outcomes. 

## Governance and Risk in AI

The journey of governance and risk control in AI may not have carried the same excitement that the services such as ChatGPT have generated, but the pathway from (1) concerns about risk, to (2) principles of ethics and trust, to (3) governance frameworks, and recently to (4) commercialised risk control offerings has been extremely fast as attempts are made to address the tidal wave of interest in this domain.

## Risk and Trust Framework Overview

There are many obvious and well discussed potential issues that jump to mind with GenAI that include:

- **data loss** through the use of chat-interactions in an uncontrolled context
- output containing **hallucinations or factual errors** that are undetected 
- **privacy and copyright** concerns with source data 
- **bias and discrimination** that reflect and reinforce the views of problematic source material

Following widespread discussions that have occured on these topics and the direct personal experience that many have had with these issues many companies were early to establish trust policies that attempted to address these concerns.  [Atlassian is an example](https://www.atlassian.com/trust/responsible-tech-principles) of one such organisation that was proactive here with their responsible trust principles.  Governments around the world have followed including here in Australia with the [8 AI Ethics Principles that have been created](https://www.industry.gov.au/publications/australias-artificial-intelligence-ethics-principles/australias-ai-ethics-principles):

- **Human, Societal, and Environmental Wellbeing**: AI should benefit people and the environment
- **Human-Centred Values**: AI should respect human rights, diversity, and autonomy
- **Fairness**: AI should be inclusive and not create bias or discrimination
- **Privacy Protection and Security**: AI must respect privacy and data security
- **Reliability and Safety**: AI systems should be safe and operate reliably
- **Transparency and Explainability**: AI decisions should be understandable
- **Contestability**: People should be able to challenge AI decisions
- **Accountability**: Those responsible for AI systems must be held accountable

These are similar in nature to the [Australian Privacy Principles (APPs)](https://www.oaic.gov.au/privacy/australian-privacy-principles) although the APPs are part of the Australian Privacy Act so have a regulatory backing which makes them legally enforceable. The AI Ethics principles (for now) are  voluntary guidelines in Australia.   The principles themselves are sensible and should be followed, but are not tactical in a way that a regular business can employ with ease.

## Governance and AI

As we move from principles based guidance to more practical governance and control frameworks I like the [approach presented by PWC](https://www.pwc.com/us/en/tech-effect/ai-analytics/managing-generative-ai-risks.html) as a starting point.  

![PWC AI Governance](https://toobstar.github.io/images/pwc_ai_governance.png)

It provides an overview of the key domains of governance and places them in context with each other:

- **Strategy:** The consideration of ethics and the regulatory environment
- **Control:** Processes for governance, compliance and risk management 
- **Responsible Practices:** Novel AI specific concerns such as explainability, bias and safety.  These relate most directly to the points highlighted in the AI Ethics principles framework.  
- **Core Practices:** Operational processes for identifying and managing issues specific to AI

The domain of risk control in AI have developed very quickly such that there is now an [ISO standard for AI Governance (38507)](https://www.iso.org/standard/56641.html) as well as a [NIST AI  Risk framework (AI-600-1)](https://www.nist.gov/itl/ai-risk-management-framework).  They are both (surprisingly) mature and well considered standards that would make sense to be deployed in risk adverse organisations that have embraced AI and have the capacity to manage AI risk alongside existing security frameworks such as ISO 27001, NIST, SOC etc. 

## Risk Management

Although this is a highly fluid domain the sort of novel and emerging risks that should be considered include this list shared by advisor on cyber risk [Andrew Milroy](https://www.linkedin.com/in/andrewmilroy/) at a recent event I attended:

![Emerging AI Risks](https://toobstar.github.io/images/ai-risk-examples.png)

Another practical and control focussed approach is to look at a vendor based view such as that presented by [Wiz](https://www.wiz.io/solutions/ai-spm).  At a [recent CISO conference](https://focusnetwork.co/cisoleaders.com.au/) Wiz presented an AI-pipeline with the various opportunities they have identified to apply risk controls:  

![Wiz AI Risk Control](https://toobstar.github.io/images/wiz-ai-risk-pipeline.png)

This is a very practical guide for how an organisation could detect, prevent and remediate risks that GenAI brings to operations. It brings together oversight on data, configuration and workloads specific to AI that would hope to manage emerging risks that would otherwise go by unmanaged.  Beyond the "posture management" approach there are also tools emerging to address specific risks such as [IBM's AI Bias detection capability AIF 360](https://research.ibm.com/blog/ai-fairness-360). 

I also liked this model of risks in AI presented by [EY](https://www.ey.com/en_au/services/consulting/trusted-ai-platform) that places AI risks alongside more traditional risks in the application stack:  

![Modelling AI Risks from EY](https://toobstar.github.io/images/ey-ai-risk-model.png)

There is value applying past experience on this topic and presenting AI risks alongside existing risks helps to integrate their treatment with existing processes.

Finally and most comprehensively for a complete understanding of tactics and risks related to AI the go-to frameworks of [OWASP](https://genai.owasp.org) and [Mitre Attack](https://atlas.mitre.org) now incorporate AI overviews which are as detailed as you'd expect them to be.  MIT is also maintaining an extensive database of [AI Risks](https://airisk.mit.edu) which is worth being aware of as well.

![OWASP Top 10 AI Risks](https://toobstar.github.io/images/owasp_ai_top10.png)

My focus with this article has been on *internal* risks from the use of AI.  There is significant evidence that the main "threat" from AI is from *external* bad-actors using AI to improve the effectiveness of their existing methods such as phishing using generated audio/video or harvested personal information to make their approach more credible.  For examples of exploited internal risks the examples I could find relate to privacy, data breaches or bias.  Many of the risks that have been documented above could be theoretical but it's comforting that they are being considered deeply and worth tracking these given the significant focus on this domain with such a broad variety of organisations.  




