# Make MS Edge less annoying on macOS

In the past, Edge was a good alternative to Chrome. But due to the laws of corporate thermodynmics, everything that was good once must not be allowed to exist for long. So countless product managers in Redmond have been working hard to make Edge as annoying as possible.

But due to another quirk in those dynamics, the product managers are able to force their bad ideas onto You, the freeloading user who just chooses to install Edge one day for free. But by the power of the Enterprise Gods they are forbidden from forcing their abominations onto paying customers, so they have to provide a way to disable them.

This repository enables you to channel the Enterprise Gods in order to return your installation of Edge to its former glory.

## How to use

Put `com.microsoft.Edge.plist` into `/Library/Managed Preferences` and restart Edge.

In case it isn't directly obvious if it worked, you can confirm that the policies are active by going to `edge://policy` in Edge.

## Caveats

On my unmanaged Macs, `/Library/Managed Preferences` gets wiped on every reboot.

# What will it actually do?

It will disable the following annoyances:

- Disable the "Hubs" sidebar annoyance (that's the one with the ugly icon)
- Allow you to override SSL errors
- Make sure websites have to get your permission before they can send you notifications
- Do not recommend to be the default PDF reader
- Enable you to override feature flags using `edge://flags`
- Disable Edge Workspaces
- Disable the built-in Password Manager
- Do not print PDFs as images by default
- Disable linking Microsoft accounts to Azure Active Directory accounts
- Do not show Bing suggesstions in the address bar
- Disable the Collections annonyance
- Disable the "Enhance Images" annonyance
- Disable the "Follow influencers, site or topic" annoyance
- Remove lots of annoyance from the "new tab" page, and, by default, replace it with "about:blank"
- Disable the "Shopping assistant" scam
- Disable the "reward points" scam
- Disable the "Compose" LLM text generation annoyance
- Disable the "Turing service" text prediction annoyance
- Disable "Edge Feedback", if they'd listen we wouldn't need this repo
- Disable the crypto wallet (this annoyance never made it to macOS, but we disable it anyway in case it ever does)
- Disable the ability to automatically "enhance" images on the web
- Disable participation in the "Experimentation and Configuration Service"
- Remove option to contact "support agents" from within the browser
- Remove ads for the insider program
- Remove ads for Adobe Acrobat
- Do not be "transparent" to so-called "acceptable" ads
- Do not show the "mini menu" that pops up on websites after selecting text
- Do not send "find on page" searches to Bing
- Do not "resolve" navigation errors by sending them to Bing
- Do not allow websites to query for saved payment methods
- Do not send "tab information" to Microsoft
- Never show "full-tab promotional content" to users
- When copying the URL from the address bar, copy it as plain text only
- Disable sidebar search
- Remove the ability to send your voice recordings to Azure Cognitive Services
- Don't send "diagnostic data" to Microsoft
- Never sync autofill, history, open tabs or passwords to Microsoft
- Remove cached images and files on browser exit
- Force strict tracking prevention
- Disable vertical tabs, this is not Opera
- Disable annoying reverse search on-hover menu on images
- Disable first run "experience"
- Reduce the user-agent header

If you disagree with any of these, or if you think something is missing, see [the official reference](https://learn.microsoft.com/en-gb/DeployEdge/microsoft-edge-policies) for inspiration.

Also, you can [watch this](https://github.com/MicrosoftDocs/Edge-Enterprise/commits/public/edgeenterprise/microsoft-edge-policies.md) for any new bad ideas as they come up.

## Before
![Before](https://github.com/zakx/unfuck-edge/assets/628602/07580cec-447e-4672-93f2-3e6f38627f1c)

## After
![After](https://github.com/zakx/unfuck-edge/assets/628602/1bb200bd-8710-4d2f-be42-e570f71ed0c6)
