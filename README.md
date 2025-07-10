# ADO Insights

This repository is configured to run an ADO MCP service that provides insights into Azure DevOps (ADO) projects. The service is designed to help users interact with ADO data, such as work items, builds, releases, repositories, and more.



## Getting Started
1. Update the `devcontainer.env` file accordingly.
1. Re-open the repository in a dev container to apply the changes.
1. Login to the Azure CLI:
   ```
   az login --use-device-code --allow-no-subscriptions
   ```
1. Login to the Azure DevOps CLI:
   ```
   echo $AZURE_DEVOPS_EXT_PAT | az devops login
   ```
1. Refresh the tools;
1. Select the custom chat mode "ADO Insights" in "Ask/Agent" dropdown. (optional)
1. Begin chatting with the agent of your choice about your ADO projects.

## Notes
- Run this repository in a dev container. Container-izing helps MCP sprawl as well as context for the AZ CLI and other tools.
- The MCP surface area is constantly evolving. Feel free to add new features or request changes.
- The ADO Insights chat mode was copied by hand from the current MCP tools. It is not automatically generated. If you make changes to the MCP tools, please update the chat mode accordingly.

## Example Usage
You can ask the agent questions like:
- "Give me some detailed insights about <MY_TEAM>'s last sprint"
- "What are the common themes of our open bugs?