# LangGraph Customer Support Ticket Router

A Google Colab example that routes customer support tickets with a small LangGraph workflow. It uses simple keyword rules, so it needs no LLM or API key.

## What the notebook demonstrates

- A typed state containing the original ticket, its category, and the reply.
- A classifier node that checks for billing keywords such as `charge`, `payment`, `refund`, and `invoice`. Tickets without those keywords go to the technical category.
- A conditional edge that routes each ticket to a billing or technical response node.
- A graph visualization and one example ticket for each route.

## Run in Google Colab

Open [ticket_router.ipynb](ticket_router.ipynb) in Google Colab. Run the setup cell to install LangGraph, then execute the notebook cells from top to bottom. The sample outputs show each ticket's category and generated support reply.

The keyword rules and replies are intentionally simple examples; adapt them to your support workflow as needed.
