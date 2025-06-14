# Python - MCP Random Weather

This project demonstrates a simple "random weather" server using the `mcp` library. It exposes a tool that returns a random weather condition for a given location.

MCP (Model Context Protocol) is a universal standard that enables AI agents (LLMs) to access data, tools and services. In this case, we will build a "server" that generates (random) weather data for an LLM to interact with.

## Setting Up

This project uses `uv` for package management. Go here for [instructions on how to install uv](https://docs.astral.sh/uv/getting-started/installation/).

```sh
uv venv
```

Activate the virtual environment:

```sh
source .venv/bin/activate
```

Install dependencies.

```sh
uv sync
```

## How To Run

To test the weather MCP server, execute the following command:

```sh
mcp dev src/mcp_crazy_weather.py
```

Then wait a while for to load, and click the link to "open inspector with token pre-filled". This will give you a UI you can use to test the MCP server right in your browser.

## Notes For Later

- Google Sheets MCP Server: https://github.com/xing5/mcp-google-sheets
- Follow all instructions to set up the MCP server.
- Set up Google Cloud:
  - Create a service account.
  - Service account JSON.
  - Enable Drive and Sheets API in the GCP project.
- Set up Claude desktop
- Set up MCP server with Claude desktop.
