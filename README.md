# YourAI Context

<img src="assets/logo.png" alt="YourAI fingerprint logo" width="128">

YourAI Context gives authorized employees read-only access to their recent computer activity and their organization's published knowledge library from compatible AI agents.

The plugin combines:

- a hosted, read-only MCP connector at `https://yourai.com/mcp`; and
- a routing skill that tells the agent when private organization or recent computer context can resolve a request.

## Requirements

- A YourAI organization account.
- An enrolled Context Gatherer device for recent computer activity.
- A published organization library for shared wiki and procedure searches.

## Install in Cursor or Grok Bot

After the plugin is published, find **YourAI Context** in the marketplace, choose **Install**, and complete the YourAI sign-in and consent flow when first prompted.

For local development, copy this repository to:

```text
~/.cursor/plugins/local/yourai-context
```

Then restart Cursor or run **Developer: Reload Window**.

## Example requests

- "What was I working on this morning?"
- "Tell me about the Lighthouse Blueberry review."
- "What is our vendor-onboarding process?"
- "Read the complete Project Lantern page."

## Data and oversight

The plugin contains no credentials. The client discovers YourAI OAuth from the hosted MCP server and stores the resulting authorization.

YourAI records every authenticated connector request and response, including queries and returned content, for company oversight. The connector does not receive the surrounding AI conversation. See the [YourAI Context documentation](https://yourai.com/docs/context) and [Privacy Policy](https://yourai.com/privacy) for details.

## Support

Contact [support@yourai.com](mailto:support@yourai.com) or visit [yourai.com/contact](https://yourai.com/contact).

## License

The plugin configuration and routing skill are licensed under the Apache License 2.0. The YourAI name and logo are trademarks of Melade LLC and are not licensed for third-party branding.
