# QualityMax for Cursor

Investigate failed Playwright runs recorded in QualityMax without leaving Cursor. The plugin connects Cursor to the hosted QualityMax MCP server and adds a skill for explaining a failed run from its results, logs, and available artifacts.

## Connect

1. Follow Cursor's [local plugin setup](https://cursor.com/docs/plugins#test-plugins-locally). Copy this repository's plugin files into `~/.cursor/plugins/local/qualitymax` and reload Cursor.
2. In Cursor's **Customize** view, find the plugin's QualityMax MCP server and connect it. Sign in to QualityMax when prompted.
3. Copy an execution ID from a Playwright run you can access in QualityMax.

## Try it

Paste this into Cursor Agent with your execution ID:

> Explain why Playwright execution EXECUTION_ID failed using QualityMax. Show me the failed step or assertion, the evidence for your diagnosis, and any available screenshot or trace links.

The skill reads an existing execution and points out any gaps in the evidence. See the [QualityMax MCP quickstart](https://docs.qualitymax.io/quickstart-mcp/) and the [execution tool reference](https://docs.qualitymax.io/reference/mcp/execution/#get_execution) for details.

## Support and privacy

Open a [GitHub issue](https://github.com/Quality-Max/qualitymax-cursor-plugin/issues) for plugin feedback. Leave execution logs, credentials, and private artifact links out of public issues.

This plugin sends requests to the hosted QualityMax MCP server. See the [QualityMax privacy policy](https://qualitymax.io/privacy) and [terms of use](https://qualitymax.io/legal).

The plugin source is [MIT licensed](LICENSE). QualityMax retains its rights to the QualityMax logo and trademarks.
