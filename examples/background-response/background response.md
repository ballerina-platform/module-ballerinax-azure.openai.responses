# Background Response

This example demonstrates how to create a background response and cancel it using the Azure OpenAI Responses API.

Background responses are useful for long-running or computationally intensive tasks where you don't want to wait for a synchronous response. They can be cancelled if they are no longer needed.

## Prerequisites

1. Generate an Azure OpenAI API key as described in the [setup guide](https://central.ballerina.io/ballerinax/azure.openai.responses/latest#setup-guide).

2. Create a `Config.toml` file in the `background-response` directory with the following content:

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

1. Creates a background response (`background: true`) for a long-running analysis task.
2. Cancels the background response before it completes.
3. Deletes the cancelled response to clean up.
