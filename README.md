# Gemini CLI Extension - BigQuery Conversational Analytics

> [!NOTE]
> This extension is currently in beta (pre-v1.0), and may see breaking changes until the first stable release (v1.0).

Developers can effortlessly connect, interact, and generate data insights with [BigQuery](https://cloud.google.com/bigquery/docs) datasets and data using natural language commands.

Learn more about [Gemini CLI Extensions](https://github.com/google-gemini/gemini-cli/blob/main/docs/extension.md).

## **Why Use the BigQuery Conversational Analytics Extension?**

* **Natural Language to insights :** Ask a variety of questions from your BigQuery data and generate intelligent insights.
* **Seamless Workflow:** Stay in your CLI. No need to constantly switch contexts to the GCP console for generating analytics insights. .
* **Leverage prebuilt agent :** Access to advanced insights offered by a built-in agent behind  [Conversational Analytics API](https://cloud.google.com/gemini/docs/conversational-analytics-api/overview)

## **Prerequisites**

Before you begin, ensure you have the following:

* [Gemini CLI](https://github.com/google-gemini/gemini-cli) installed with version +v0.6.0.
* A Google Cloud project with the **Data Analytics API with Gemini**, **Gemini for Google Cloud API** and **BigQuery API** enabled.
* IAM Roles:
     * BigQuery User (`roles/bigquery.user`) (for executing queries and view metadata)
     * Gemini for Google Cloud (`roles/cloudaicompanion.user`) (to use the conversational analytics API)

## Installation

To install the extension, use the command:

```bash
gemini extensions install github.com/gemini-cli-extensions/bigquery-conversational-analytics
```

## Configuration

Set the following environment variables before starting the Gemini CLI:

*   `BIGQUERY_PROJECT`: The GCP project ID.
*   `BIGQUERY_LOCATION`: (Optional) The dataset location.
*   `BIGQUERY_USE_CLIENT_OAUTH`: (Optional) Set to `true` to use client-side OAuth for authorization.

Ensure [Application Default Credentials](https://cloud.google.com/docs/authentication/gcloud) are available in your environment.

## **Usage Examples**

Interact with BigQuery using natural language right from your IDE:

* **Ask for insights**

  * Using the tables under bigquery-public-data.google\_analytics\_sample , tell me the channels I should focus on and why?

## **Supported Tools**

This extension provides a comprehensive set of tools:

* `ask_data_insights`: Executes a SQL query.
* `search_catalog`: Find BigQuery tables relevant to users, natural language query.

## Additional Extensions

Find additional extensions to support your entire software development lifecycle at [github.com/gemini-cli-extensions](https://github.com/gemini-cli-extensions).

## Troubleshooting

* "cannot execute binary file": Ensure the correct binary for your OS/Architecture has been downloaded. See [Installing the server](https://googleapis.github.io/genai-toolbox/getting-started/introduction/#installing-the-server) for more information.
