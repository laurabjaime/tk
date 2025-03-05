# Send Python Code to Taktile API

This GitHub Action automatically triggers Taktile API to update code nodes when a merge to the `main` branch occurs.

## Features
✅ Automatically detects `.py` files in the repository  
✅ Reads and processes Python files dynamically  
✅ Retrieves `flow_id` and `node_id` dynamically from the API  
✅ Sends API requests using GitHub Actions  

## How to Set Up

1. Fork this repository or add it to your GitHub
2. Set up GitHub Secrets in your repository:
   - `API_KEY`: Your API authentication key
   - `ORG_NAME`: The name of the organization used in the API
3. Push Python files to the repository.
4. Merge to `main`, and the action will automatically send the code to the API!

## Example Usage
Whenever a Python file is updated and merged to `main`, the workflow runs automatically and update the code nodes with same name from Taktile.

## Important notes
- Ensure your .py files names match the code_node names on Taktile
- If a file is empty, it will be skipped with a warning
- If no Python files are found, the workflow will stop
