# thirdweb Engine Deploy Locally

Let's deploy thirdweb Engine locally in easiest way possible. This repository is maintained by thirdweb community team.

> [!WARNING]
> Use this for demo / preview purposes only. This is not recommended for production use. If you wanna use thirdweb Engine in production, try [cloud-hosted version](https://thirdweb.com/dashboard/engine?requestCloudHosted) or deploy a [self-hosted version](https://support.thirdweb.com/infrastructure/eRgkLPBdL1WJJLzAbuWrPZ/how-to-deploy-your-self-hosted-thirdweb-engine-on-the-railway/d97FnFt8e926FqniTaYxfD).

## Requirements

- [Docker](https://docs.docker.com/get-docker/)
- [NodeJS](https://nodejs.org/en/download/)
- [Postgres](https://postgresql.org/download/) (only supports v14+)
- [Redis](https://redis.io/downloads/) (only supports v7.2.4+)
- [thirdweb API secret key](https://thirdweb.com/dashboard/api-keys)
- [Wallet address](https://portal.thirdweb.com/glossary/wallet)

## Usage

1. Clone the repository.
2. Configure the `.env.example` file with your API secret key, wallet address, and ngrok auth token.
3. Start Docker on your local machine.
4. Run `npm run start` to deploy the engine locally, wait for it to finish.
5. A new tab will open in your browser if you provided ngrok auth token in the `.env` file.
   - This will be your ngrok URL to access the engine from anywhere. You can use this URL to import it to your thirdweb dashboard.
6. If not, visit `https://localhost:3005` in your browser.
7. That's it!

For detailed guide, visit [here](https://support.thirdweb.com/infrastructure/eRgkLPBdL1WJJLzAbuWrPZ/how-to-deploy-thirdweb-engine-to-your-local-machine/nhgkjfQ7S9b6Hbe1dp9uuh).

> [!NOTE]
> We recommend to use the versioned image instead of `latest` tag in the `docker-compose.yml` file. You can find the versioned image list in the [Docker Hub](https://hub.docker.com/r/thirdweb/engine).

## Get Help

- [Documentation](https://portal.thirdweb.com)
- [Submit a ticket](https://support.thirdweb.com)
- [Join Discord](https://discord.gg/thirdweb)
