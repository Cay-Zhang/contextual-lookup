<div align="center">

<img src="https://github.com/user-attachments/assets/4dd2dc90-ccef-4533-8118-adfaa2dec7de" width="80" height="80">

# Contextual Lookup
[Demo on YouTube](https://youtu.be/3iORsVBdQR8)

</div>

> **ℹ️ Welcome to the Support Hub for Contextual Lookup!**
>
> This repository is dedicated to the **Privacy Policy** and **Issue Tracking** (bug reports, feature requests) for the Contextual Lookup Chrome extension.
>
> **Please note: The source code for the extension is <u>not</u> hosted in this repository.**

## Privacy Policy

Your privacy is important to us. You can find the full Privacy Policy for the Contextual Lookup Chrome extension here:

➡️ **[View the Privacy Policy](./PRIVACY_POLICY.md)**

## Issue Tracking & Support

Encountered a bug? Have a great idea for a new feature? Need clarification on something?
* **Search Existing Issues:** Before submitting, please check if a similar issue or request has already been reported [here](https://github.com/Cay-Zhang/contextual-lookup/issues).
* **Create a New Issue:** If not, please [open a new issue](https://github.com/Cay-Zhang/contextual-lookup/issues/new/choose), providing as much detail as possible (e.g., steps to reproduce, browser version, expected behavior vs. actual behavior).

We appreciate your feedback and contributions to improving Contextual Lookup!

## About Contextual Lookup

Below is information regarding the Contextual Lookup Chrome extension itself.

### Overview
Navigating technical jargon, complex topics, or unfamiliar acronyms can be challenging, especially when conventional lookup methods fail to consider the surrounding context.
Contextual Lookup is a Chrome extension that addresses this gap by extracting and using contextual information like surrounding text, page metadata, and more, delivering tailored and relevant insights directly within the browser.

Built with the latest web technologies, Contextual Lookup offers a seamless user experience while providing flexibility with multiple AI integration options, including Chrome's native AI models and server-side solutions via OpenRouter.

### Installation
The Contextual Lookup extension can be installed from the Chrome Web Store:

➡️ **[Install from Chrome Web Store](https://chromewebstore.google.com/detail/contextual-lookup/icbalolgoiagfcfggefkjloconikgmon?utm_source=github&utm_medium=readme)**

To use the **built-in AI model**, ensure Chrome flags are configured as below:
1.  `chrome://flags/#optimization-guide-on-device-model` set to `Enabled BypassPerfRequirement`
2.  `chrome://flags/#text-safety-classifier` set to `Disabled`
3.  `chrome://flags/#prompt-api-for-gemini-nano` set to `Enabled`

To use **server-side models**, enter an OpenRouter API key in the extension **popup** (not the settings page).

### Usage
**Contextual Lookup** enhances the lookup experience by integrating relevant contextual information, such as surrounding text, page URL, and tab title, into the context of language models. Here’s how it works:

- **Selecting and Hovering**: Users can select text or code and hover over the thin bar that appears below the selection. The bar will gradually expand into the definition popover in a short time span.
- **Tailored Responses Based on Selection**:
    - For **words or phrases**, the definition popover displays the meaning in context and includes one relevant example sentence.
    - For **acronyms**, it shows the expanded form and a concise, Wikipedia-style definition.
    - For **code**, it explains the effect of the selection in context and provides one illustrative code snippet.
- **Model Options**: Users can choose between Chrome's built-in AI model (browser support required) or server-side models like Gemini 1.5 Pro and Gemini 1.5 Flash-8B (OpenRouter API key required).
- **Contextual Search**: If the contextual definition isn’t satisfactory, users can click the search button in the popover. The extension generates a context-aware search query and opens a Google search page.
- **Acronym Detection**: Acronyms are automatically highlighted on web pages if the feature is enabled. Hovering over them activates the lookup function, streamlining understanding of domain-specific abbreviations.
