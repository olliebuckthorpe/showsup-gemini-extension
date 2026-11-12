# ShowsUp for Gemini CLI

Connects [Gemini CLI](https://github.com/google-gemini/gemini-cli) to your [ShowsUp](https://showsup.ai) account. ShowsUp sends reminders by email, SMS, WhatsApp and voice before sales meetings, and helps recover no-shows.

Ask in plain language:

- "What meetings do I have this week?"
- "Which prospects haven't confirmed their meeting yet?"
- "Which of my reminder sequences are switched on?"

## Install

```bash
gemini extensions install https://github.com/olliebuckthorpe/showsup-gemini-extension
```

You need a ShowsUp account; the free plan works. The first time Gemini uses ShowsUp, your browser opens ShowsUp's sign-in page. Choose which permissions to grant and select **Allow**. There is no API key to copy.

## What it can do

The extension connects to the ShowsUp MCP server at `https://api.showsup.ai/mcp`. It can read your meetings, prospects, reminder sequences, templates, review queue and account settings, and prepare changes to them.

Anything that would reach a prospect, such as sending a message, cancelling or rescheduling a meeting, or changing reminders for meetings already booked, does not run straight away. It waits on the [Approvals page](https://app.showsup.ai/approvals) until you approve it.

Reply text read from your Gmail or Outlook mailbox is never sent to Gemini.

## Disconnect

In ShowsUp, go to **Settings → Integrations → AI connections** and select **Revoke** next to Gemini. To remove the extension:

```bash
gemini extensions uninstall showsup
```

## Links

- Documentation: https://showsup.ai/docs/ai-assistants
- Privacy policy: https://showsup.ai/privacy
- Terms: https://showsup.ai/terms
- Support: support@showsup.ai

ShowsUp is a product of Pipeline Engine Ltd.
