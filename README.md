# MCT Hub

MCT Hub is a static web front end for a Copilot Studio agent that answers Microsoft Certified Trainer (MCT) Program questions.

## Site

- Production URL: <https://mcthub.z12.web.core.windows.net/>
- Static website host: Azure Storage account `mcthub`
- Source files: `src/`

## Deployment

GitHub Actions deploys the static site to the Azure Storage `$web` container when changes are pushed to `main`.

Required repository secret:

- `AZURE_STORAGE_CONNECTION_STRING`: connection string for the Azure Storage account that hosts the static website.

Manual deployment is also available from the **Actions** tab via **Deploy MCT Hub** → **Run workflow**.

## Files

- `src/index.html`: MCT Hub static web page
- `src/mcthub-logo.png`: site and agent logo asset
