# Action Repo

This repository is configured to trigger GitHub webhooks for the following events:

-   Push
-   Pull Request
-   Merge 

These webhooks send event data to a corresponding Flask application (`webhook-repo`) that processes and stores the data in a local MongoDB database.


## Webhook Configuration

The webhook is configured in the repository's settings to send payloads to the following URL:

`https://related-muskox-ace.ngrok-free.app/webhook` (forwarded from a local port using Ngrok)  

## How to Use (For Testing)

1. Clone this repository to your local machine.
2. Make changes, commit them, and push to different branches.
3. Create pull requests and merge them.
4. Observe the data being processed and displayed by the `webhook-repo` application.

## Related Repository

The backend application that receives and processes the webhook events is located in the `webhook-repo` repository:


## Note

This repository is primarily for testing purposes.
