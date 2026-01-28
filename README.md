# Gemini CLI Extension - BigQuery Conversational Analytics

> [!NOTE]
> This extension is currently in beta (pre-v1.0), and may see breaking changes until the first stable release (v1.0).

Developers can effortlessly connect, interact, and generate data insights with [BigQuery](https://cloud.google.com/bigquery/docs) datasets and data using natural language commands.

Learn more about [Gemini CLI Extensions](https://github.com/google-gemini/gemini-cli/blob/main/docs/extensions/index.md).
> [!IMPORTANT]
> **We Want Your Feedback!**
> Please share your thoughts with us by filling out our feedback [form][form]. 
> Your input is invaluable and helps us improve the project for everyone.

[form]: https://docs.google.com/forms/d/e/1FAIpQLSfEGmLR46iipyNTgwTmIDJqzkAwDPXxbocpXpUbHXydiN1RTw/viewform?usp=pp_url&entry.157487=bigquery-conversational-analytics

## **Why Use the BigQuery Conversational Analytics Extension?**

* **Natural Language to insights :** Ask a variety of questions from your BigQuery data and generate intelligent insights.
* **Seamless Workflow:** Stay in your CLI. No need to constantly switch contexts to the GCP console for generating analytics insights. .
* **Leverage prebuilt agent :** Access to advanced insights offered by a built-in agent behind  [Conversational Analytics API](https://cloud.google.com/gemini/docs/conversational-analytics-api/overview)

## Prerequisites

Before you begin, ensure you have the following:

* [Gemini CLI](https://github.com/google-gemini/gemini-cli) installed with version **+v0.6.0**.
* Setup Gemini CLI [Authentication](https://github.com/google-gemini/gemini-cli/tree/main?tab=readme-ov-file#-authentication-options).
* A Google Cloud project with the **Data Analytics API with Gemini**, **Gemini for Google Cloud API** and **BigQuery API** enabled.
* Ensure [Application Default Credentials](https://cloud.google.com/docs/authentication/gcloud) are available in your environment.
* IAM Roles:
     * BigQuery User (`roles/bigquery.user`) (for executing queries and view metadata)
     * Gemini for Google Cloud (`roles/cloudaicompanion.user`) (to use the conversational analytics API)

## Getting Started

### Installation

To install the extension, use the command:

```bash
gemini extensions install https://github.com/gemini-cli-extensions/bigquery-conversational-analytics
```

### Configuration

Set the following environment variables before starting the Gemini CLI. These variables can be loaded from a `.env` file.

```bash
export BIGQUERY_PROJECT="<your-gcp-project-id>"
export BIGQUERY_LOCATION="<your-dataset-location>"  # Optional
```

Ensure [Application Default Credentials](https://cloud.google.com/docs/authentication/gcloud) are available in your environment.

### Start Gemini CLI

To start the Gemini CLI, use the following command:

```bash
gemini
```

## Usage Examples

Interact with BigQuery using natural language right from your IDE:

* Ask for insights

  * Using the tables under bigquery-public-data.google\_analytics\_sample , tell me the channels I should focus on and why?

## Supported Tools

This extension provides a comprehensive set of tools:

* `ask_data_insights`: Perform data analysis, get insights, or answer complex questions about the contents of specific BigQuery tables.
* `search_catalog`: Find BigQuery tables relevant to users, natural language query.

## Additional Extensions

Find additional extensions to support your entire software development lifecycle at [github.com/gemini-cli-extensions](https://github.com/gemini-cli-extensions), including:
* [BigQuery Data Analytics](https://github.com/gemini-cli-extensions/bigquery-data-analytics)
* and more!

## Troubleshooting

Use `gemini --debug` to enable debugging.

Common issues:

* "failed to find default credentials: google: could not find default credentials.": Ensure [Application Default Credentials](https://cloud.google.com/docs/authentication/gcloud) are available in your environment. See [Set up Application Default Credentials](https://cloud.google.com/docs/authentication/external/set-up-adc) for more information.
* "✖ Error during discovery for server: MCP error -32000: Connection closed": The database connection has not been established. Ensure your configuration is set via environment variables.
* "✖ MCP ERROR: Error: spawn /Users/USER/.gemini/extensions/bigquery-conversational-analytics/toolbox ENOENT": The Toolbox binary did not download correctly. Ensure you are using Gemini CLI v0.6.0+.
* "cannot execute binary file": The Toolbox binary did not download correctly. Ensure the correct binary for your OS/Architecture has been downloaded. See [Installing the server](https://googleapis.github.io/genai-toolbox/getting-started/introduction/#installing-the-server) for more information.
