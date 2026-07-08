# TaskFlow API Documentation

Public-facing documentation for TaskFlow, a simple task management API — built with Mintlify as part of a technical writing assessment.

📄 **Live documentation**: https://liviazeviani.mintlify.site

## What's inside

| Section | Purpose |
| --- | --- |
| **Introduction** | What TaskFlow is, core concepts (Projects and Tasks), base URL, and expected server behavior |
| **Quickstart** | A complete first session: create a project, create a task, list, update, and delete |
| **Authentication** | How bearer authentication works and how to troubleshoot common `401` causes |
| **Error Handling** | The shared error format, every status code with real response examples, and how to fix each case |
| **API Reference** | All five endpoints, generated directly from the OpenAPI spec, with an interactive playground |

## Running locally

Install the Mintlify CLI and start the dev server from the repository root:

```bash
npm i -g mint
mint dev
```

The site will be available at `http://localhost:3000`, with live reload on every save.

## Process and decisions

**Process**: I started setting up Mintlify project, defined the structure, wrote the guide pages, and configured the API Reference to be generated directly from the OpenAPI spec.
I tested the endpoints using Postman to verify that the responses and error messages matched what I had documented.

**Structure and content**: I split the docs into two tabs, Guides and API Reference, because the two audiences read differently: new users need a step-by-step path, while experienced users just need to look up specific details.
The Quickstart covers the full workflow: create a project, create a task, list, update, delete.
Authentication and Error Handling have their own pages because they apply to every endpoint. The error page shows the error format, all status codes with real examples, and how to fix each one.

**Challenges and what I'd do differently**: I had trouble with the docs.json navigation schema: while refactoring it, I broke the site navigation, but recovered by restoring a previous version from the git history. I did everything through the Mintlify web editor, and it would have been better practice to work directly with git — editing locally and writing proper commit messages for each change, which also makes it easier to recover from mistakes like this one.

I used Claude as an AI assistant throughout the project — reviewing the site for gaps, discussing structure decisions, drafting content that I then revised, and polishing my English. It also helped me troubleshoot the bearer token authentication in Postman while I tested the API.

## Credits

- Favicon: [API icons created by rukanicon — Flaticon](https://www.flaticon.com/br/icones-gratis/api)
- AI assistance: [Claude](https://claude.ai) (Anthropic)
