# Simple Response

This example demonstrates how to create, retrieve, and list input items for a model response using the Azure OpenAI Responses API.

## Prerequisites

1. Generate an Azure OpenAI API key as described in the [setup guide](https://central.ballerina.io/ballerinax/azure.openai.responses/latest#setup-guide).

2. Create a `Config.toml` file in the `simple-response` directory with the following content:

    ```toml
    token = "<Azure OpenAI API Key>"
    serviceUrl = "<Azure OpenAI Endpoint URL>"
    ```

## Run the example

Execute the following commands to build and run the example:

```bash
bal run
```

## What this example does

1. Creates a model response asking the model to explain the Ballerina programming language.
2. Retrieves the created response by its ID to confirm it was stored.
3. Lists the input items associated with the response.
