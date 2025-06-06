# Session delivery resources

The following resources are intended for a presenter to learn and deliver the session.

We're glad you are here and look forward to your delivery of this amazing content. As an experienced presenter, we know you know HOW to present so this guide will focus on WHAT you need to present. It will provide you a full run-through of the presentation created by the presentation design team.

Along with the video of the presentation, this document will link to all the assets you need to successfully present including PowerPoint slides and demo instructions & code.

## Presentation

### Powerpoint

Download the English version of the Powerpoint Presentation from [aka.ms/AArxlk6](https://aka.ms/AArxlk6). Speaker notes are available on each slide.

### PowerPoint Slides in Additional Languages

| Language  | Last Updated |
| ------------- | ------------- |
| [Spanish](https://aka.ms/AAs7mfz)  | 2024.09.11  |
| [Portuguese](https://aka.ms/AAs7eu0) | 2024.09.11  |
| [Korean](https://aka.ms/AAv6jj9) | 2025.04.08  |
| [Japanese](https://aka.ms/AAvcauo) | 2025.04.08  |

### Video recording

[Watch the recording](https://aka.ms/AArzolk)

⚠️ In the "User Auth" section, the slides describe using Bicep to set up a federated identity credential for the Entra application. As of 12/18/2024, that feature is now in public preview, so developers can start trying it out now. It wasn't yet available when we first did the recording, however.

### Timing

Total time is allotted for the presentation, including demos, is 45 minutes.
No time for questions is budgeted into the 45 minutes.

| Segment             | Time |
|---------------------|------|
| Introduction        | 05:00 |
| AI Safety           | 06:00 |
| Keyless Auth        | 08:00 |
| User Auth           | 10:00 |
| Network Security    | 08:00 |
| Continuous Security | 06:00 |
| Wrap-up             | 02:00 |

## Demos

These are the demos that you may choose to do in the presentation. You may leave some out depending on time constraints.

### Setup

To be able to show the demos yourself, setup these two repositories:

* **AI Chat App with Built-in Auth**:
  Follow deployment instructions in [openai-chat-app-entra-auth-builtin](https://github.com/Azure-Samples/openai-chat-app-entra-auth-builtin) with the Entra ID option (not Entra External ID option).
  You must use a tenant that allows the creation of App Registrations (i.e. not the main Microsoft tenant).
  If you have a capacity constraints with OpenAI TPM quota, then set the capacity before deployment with:
  
  ```shell
  azd env set AZURE_OPENAI_DEPLOYMENT_CAPACITY 8
  ```
  
* **RAG App with Data Access Control**:
    1. Follow deployment instructions in [azure-search-openai-demo](https://github.com/Azure-Samples/azure-search-openai-demo).
    2. Enable these two optional features:
       * [User Auth with Data Access Control](https://github.com/Azure-Samples/azure-search-openai-demo/blob/main/docs/login_and_acl.md): You will need to use a tenant that allows the creation of App Registrations (not the main Microsoft tenant)
       * [User document upload](https://github.com/Azure-Samples/azure-search-openai-demo/blob/main/docs/deploy_features.md#enabling-user-document-upload)
    3. Upload a document that you can ask a question about

### Transcript

A suggested transcript for each demo is [available](https://aka.ms/AAruyl1).

### Video recordings

If you'd like, there are videos available for each demo. You can either narrate the silent version of the video, or play the video with audio.

| Demo                    | Duration | Video - Silent | Video - Audio |
| ------------------------|----------|---------------- |  ----------- |
| 1 - Built-in Auth       | 1:00     | [aka.ms/AAruqx1](https://aka.ms/AAruqx1) | [aka.ms/AAruj63](https://aka.ms/AAruj63) |
| 2 - Data Access Control | 1:45     | [aka.ms/AAruykw](https://aka.ms/AAruykw) | [aka.ms/AAruqxg](https://aka.ms/AAruqxg) |


## Change Log

Here is a log of changes made to this file:

| Date  | Changes |
| ------------- | ------------- |
| 2024.09.11 | Added change log, added Spanish and Portuguese language slide decks  |
