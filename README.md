# Securing AI Apps on Azure

*If you will be delivering this session, consult the [session-delivery-resources](./session-delivery-resources/README.md) guide for slides, demo scripts, and other resources.*

## Session Desciption

An overview of the best practices for deploying AI applications to Azure. Learn how to use managed identity (passwordless) authentication for Azure AI services. Find out how easily you can add user authentication using Microsoft Entra and built-in authentication. Explore approaches for AI safety, like Content Safety filters and Jailbreak detection. See how an AI app can be deployed safely inside a virtual network and accessible only via private endpoints.  Discover how easy it is to use CI/CD and Microsoft Defender to stay ahead of security issues in your codebases.

## Learning Outcomes

* Azure AI Content Safety filters, jailbreak detection
* Managed Identity (Keyless Auth) for Azure AI services
* User authentication with Microsoft Entra and Built-in Authentication
* Deploying AI apps inside a virtual network
* GitHub Actions with PSRules audit
* Microsoft Defender for security alerts

## Technology Used

* Azure AI
* Microsoft Entra
* Microsoft Defender
* Azure Container Apps
* Bicep
* GitHub Actions

## Additional Resources and Continued Learning

* [Microsoft Responsible AI](https://www.microsoft.com/ai/responsible-ai)
* [Azure AI Content Safety](https://aka.ms/aicontentsafety)
* [Hidden Layer Model Scanner](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/hiddenlayerinc1690422428200.hiddenlayer-model-scanner?tab=Overview)
* [Microsoft Entra developer center](https://aka.ms/dev/ms-entra)
* [Well-Architected Framework](https://aka.ms/wellarchitectedframework)
* [PSRules action for GitHub](https://github.com/microsoft/ps-rule)
* [Microsoft Defender](https://aka.ms/enable-defender)
* [Python risk identification tool for generative AI](https://aka.ms/pyrit)

Samples:

* [AI Chat App with Managed Identity (Python)](https://aka.ms/keyless-azure-containerapps)
* [AI Chat App with User Login and Built-in Auth](aka.ms/azai/auth-builtin)
* [RAG app with Azure AI Search, Data Access Control, Private Network Deployment](https://aka.ms/ragchat)

## Responsible AI

Microsoft is committed to helping our customers use our AI products responsibly, sharing our learnings, and building trust-based partnerships through tools like Transparency Notes and Impact Assessments. Many of these resources can be found at [aka.ms/RAI](https://aka.ms/RAI). Microsoft’s approach to responsible AI is grounded in our AI principles of fairness, reliability and safety, privacy and security, inclusiveness, transparency, and accountability.

Large-scale natural language, image, and speech models - like the ones used in this sample - can potentially behave in ways that are unfair, unreliable, or offensive, in turn causing harms. Please consult the [Azure OpenAI service Transparency note](https://learn.microsoft.com/legal/cognitive-services/openai/transparency-note?tabs=text) to be informed about risks and limitations.

The recommended approach to mitigating these risks is to include a safety system in your architecture that can detect and prevent harmful behavior. [Azure AI Content Safety](https://learn.microsoft.com/azure/ai-services/content-safety/overview) provides an independent layer of protection, able to detect harmful user-generated and AI-generated content in applications and services. Azure AI Content Safety includes text and image APIs that allow you to detect material that is harmful. We also have an interactive Content Safety Studio that allows you to view, explore and try out sample code for detecting harmful content across different modalities. The following [quickstart documentation](https://learn.microsoft.com/azure/ai-services/content-safety/quickstart-text?tabs=visual-studio%2Clinux&pivots=programming-language-rest) guides you through making requests to the service.

Another aspect to take into account is the overall application performance. With multi-modal and multi-models applications, we consider performance to mean that the system performs as you and your users expect, including not generating harmful outputs. It's important to assess the performance of your overall application using [Performance and Quality and Risk and Safety evaluators.](https://learn.microsoft.com/en-us/azure/ai-studio/concepts/evaluation-metrics-built-in?tabs=warning)  You also have the ability to create and evaluate with [custom evaluators.](https://learn.microsoft.com/en-us/azure/ai-studio/how-to/develop/evaluate-sdk#custom-evaluators)

You can evaluate your AI application in your development environment using the [Azure AI Evaluation SDK.](https://microsoft.github.io/promptflow/index.html) Given either a test dataset or a target, your generative AI application generations are quantitatively measured with built-in evaluators or custom evaluators of your choice. To get started with the prompt flow sdk to evaluate your system, you can follow the [quickstart guide.](https://learn.microsoft.com/azure/ai-studio/how-to/develop/flow-evaluate-sdk) Once you execute an evaluation run, you can [visualize the results in Azure AI Studio.](https://learn.microsoft.com/azure/ai-studio/how-to/evaluate-flow-results)

## Content Owners

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->

<table>
   <tr>
    <td align="center"><a href="https://developer.microsoft.com/advocates/pamela-fox">
        <img src="https://developer.microsoft.com/en-us/advocates/media/profiles/pamela-fox.png" width="100px;" alt="Pamela Fox"/><br />
        <sub><strong>PAMELA FOX</strong></sub></a><br />
         <a href="https://github.com/pamelafox" title="GitHub profile for Pamela">📢</a>
    </td>
    <td align="center"><a href="https://developer.microsoft.com/advocates/sarah-young">
        <img src="https://developer.microsoft.com/en-us/advocates/media/profiles/sarah-young.png" width="100px;" alt="Sarah Young"/><br />
        <sub><strong>SARAH YOUNG</strong></sub></a><br />
         <a href="https://github.com/sarah-yo" title="GitHub profile for Sarah">📢</a>
    </td>
</tr></table>
