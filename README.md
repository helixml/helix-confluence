# helix-confluence

This project helps you deploy the Helix app for Confluence so that you can talk to your Confluence instance with natural language, and ask questions like:

1. Show me the documents owned by me, Adam Fox
2. Display the documents last edited by Bob Gelder


## Setup

   ```
1. Go to [https://app.tryhelix.ai/account](https://app.tryhelix.ai/account) or the corresponding domain for your private Helix deployment and run the "CLI install & login" section, e.g:
   export HELIX_URL=...
   export HELIX_API_KEY=
   ```

2. Copy the example environment file:
   ```
   cp .env.example .env
   ```

3. Edit `.env` and add your Jira information:
   ```
   JIRA_HOSTNAME=https://yourco.atlassian.net
   JIRA_API_EMAIL=you@domain.com
   JIRA_API_KEY=your_jira_api_key_here
   ```
   Replace the values with your actual Jira instance details and API key.


## Deployment

To deploy the Helix JIRA app:

```
bash deploy.sh
```

This script will process your configuration and test it using Helix.

