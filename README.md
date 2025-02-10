# How to build an AI agent with Safe and LangChain

This example repo shows how to create an AI agent with capabilities to interact with your Safe. Please read [Create an AI agent that can interact with your Safe](https://docs.safe.global/home/ai-agent-setup) to see how this app was created.

## What you’ll need

**Prerequisite knowledge:** You will need some basic familiarity with the [LangChain framework](https://www.langchain.com/langchain) and [Node.js](https://nodejs.org/en).

Before progressing with the tutorial, please make sure you have:

- Installed and opened `ollama`. This tutorial will run [`mistral-nemo`](https://ollama.com/library/mistral-nemo) (minimum 16GB RAM & 8GB disk space required), but feel free to explore [other models](https://ollama.com/library);
- Set up a wallet for your agent with some Sepolia test funds to pay for the transactions, for example with [Metamask](https://metamask.io/);
- (Optional) If you wish to use OpenAI models instead (or another provider), you will need to create an account on their website and get an API key;
- (Optional) Set up an account on [LangSmith](https://smith.langchain.com/) for agent observability & monitoring.

## Getting Started

To install this example application, run the following commands:

```bash
git clone https://github.com/5afe/safe-ai-agent-tutorial.git
cd safe-ai-agent-tutorial
pnpm i
```

This will get a copy of the project installed locally. Now, create a file named `.env.local` at the root of your project, and add your private key and address key to it:

```bash
cp .env.example .env.local
```

Run the agent locally with the following command:

```bash
pnpm start
```

See the resulting output in your terminal. You should see the agent interacting with your Safe. For more information on what is going on under the hood, set up an account on [LangSmith](https://smith.langchain.com/) and monitor your agent's activity.

## Help

Please post any questions on [Stack Exchange](https://ethereum.stackexchange.com/questions/tagged/safe-core) with the `safe-core` tag.

## License

MIT, see [LICENSE](LICENSE).
