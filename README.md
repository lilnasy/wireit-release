# Wireit Release Automation

This repository contains a scheduled GitHub Actions workflow that automates the process of creating a release for the npm package "wireit" with all dependencies bundled in.

## How to Use This Repository

1. Clone this repository:
   ```sh
   git clone https://github.com/githubnext/workspace-blank.git
   cd workspace-blank
   ```

2. Make sure you have the necessary permissions to create and publish releases on GitHub.

3. The workflow will automatically run according to the defined schedule. You can also manually trigger the workflow if needed.

## How to Run the Scheduled GitHub Actions Workflow

The GitHub Actions workflow is defined in the `.github/workflows/release.yml` file. It is configured to run on a schedule, but you can also trigger it manually.

To manually trigger the workflow:

1. Go to the "Actions" tab of your repository on GitHub.
2. Select the "Release" workflow from the list of workflows.
3. Click the "Run workflow" button and follow the prompts.

The workflow will perform the following steps:

1. Clone the `github.com/google/wireit` repository.
2. Create and configure the necessary files (`pnpm-workspace.yaml`, `.npmrc`, `package.json`).
3. Install dependencies and publish the package.
