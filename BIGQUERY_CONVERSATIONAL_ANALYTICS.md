
## BigQuery Conversational Analytics MCP Server 

This section covers connecting to a BigQuery instance.

1.  **Verify Environment Variables**: Before attempting to connect, confirm with the user that the following environment variables are set in the extension configuration or their shell environment.

    * `BIGQUERY_PROJECT`: The GCP project ID.

2.  **Handle Missing Variables**: If a command fails with an error message containing a placeholder like `${BIGQUERY_PROJECT}`, it signifies a missing environment variable. Inform the user which variable is missing and instruct them to set it.

3.  **Handle Permission Errors**:
    * For operations that execute queries and view metadata, the user needs the
      **BigQuery User** (`roles/bigquery.user`) and **BigQuery Metadata Viewer** (`roles/bigquery.metadataViewer`) role.
    * For operations that create, or modify datasets and tables, the user needs
      the **BigQuery Data Editor** (`roles/bigquery.dataEditor`) role.
    * For operations that perform data analysis or get insights, the user needs **Gemini Data Analytics Stateless Chat User** (`roles/geminidataanalytics.dataAgentStatelessUser`) role.
    * If an operation fails due to permissions, identify the type of operation
      and recommend the appropriate role. you can provide these links for
      assistance:
        *   Granting Roles: https://cloud.google.com/iam/docs/grant-role-console
        *   BigQuery Roles and Permissions: https://cloud.google.com/iam/docs/roles-permissions/bigquery
        *   Conversational Analytics API Roles and Permissions: https://cloud.google.com/gemini/docs/conversational-analytics-api/access-control
