# Composable CDP Prototype

A prototype developed to show how a composable Customer Data Platform (CDP) is put together, and how a marketer builds an audience on top of it.

> **This is a prototype.** It uses fictional data (a made-up pet-food retailer) and has no live systems, customers or vendors behind it. It was built to demonstrate design thinking, not to run in production.

## What is in this repository

| File | What it is |
|---|---|
| `index.html` | Architecture overview: the layers of a composable CDP, how an audience gets created, and where to buy versus build. |
| `audience-composer.html` | Interactive audience builder. Changing any control regenerates the audience definition (JSON), illustrative SQL and an execution plan. |

Both are plain HTML, CSS and JavaScript. There is nothing to install and no build step.

## Run it

Open `index.html` in any browser. To serve it locally instead:

```
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## What it demonstrates

- How the layers of a composable CDP fit together
- Real-time, batch and hybrid audiences, and why each exists
- How a marketer's choices become a structured definition and an execution plan
- Trade-offs between buying tools and building components
- Guardrails (validation warnings) that catch risky set-ups before launch

## Related projects (separate, not part of this repository)

This is an independent design and UI prototype. It is not connected to my other CDP work, such as the working AWS-based Pet Food CDP. Those projects are built and deployed on AWS. This one describes a different, composable architecture and has no running backend. The fictional pet-food retailer is only a shared example theme.

## What a real build would still need

Identity resolution, roles and approvals, safe editing of a live audience, connector set-up and rate limits, a consent management interface, and cost controls for streaming jobs.
