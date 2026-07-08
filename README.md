# TaskFlow API Documentation

Public-facing documentation for TaskFlow, a simple task management API — built with Mintlify as part of a technical writing assessment.

📄 Live documentation: https://liviazeviani.mintlify.site

What's inside

**📄 Live documentation:** https://liviazeviani.mintlify.site

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



