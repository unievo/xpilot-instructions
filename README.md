# xPilot Instructions

This repository is a library of instructions for xPilot or other AI agents. Its purpose is to provide up to date information on any topic usable in AI contexts, such as APIs, tools, tool usage, coding guidelines, rules and best practices, networks, network interaction, smart contracts, dapps, templates, SDKs, etc., for automations, app development, testing, deploying, etc.

## Structure

Instructions are provided in the form of markdown files, and are organized into a structure that allows for easy file navigation and retrieval. Each topic has its own directory, which contains only `table of contents` files, and a `content` subdirectory with files for detailed information on topic subjects.

Table of contents files briefly describe available topics and topic subjects, and contain links to detailed instruction files under the content subdirectory.

### Example:

```markdown
MultiversX/
├── tools/                                  <-- General topic directory
│   ├── mxpy/                               <-- Specific topic directory
│   │   ├── Network Operations.md           <-- Table of contents file
│   │   ├── Validator Operations.md         <-- Table of contents file
│   │   └── content/                        <-- Content details directory
│   │       ├── tx/                         <-- Subject instructions directory
│   │       │   ├── mxpy-tx-new.md          <-- Subject instructions file
│   │       │   ├── mxpy-tx-send.md         <-- Subject instructions file
│   │       │   └── ...                     ...
│   │       ├── validator/
│   │       │   ├── mxpy-validator-stake.md
│   │       │   └── ...
│   │       ...
│   │
│   ├── sc-meta/
│   │   ├── ...
│   │   ...
│   │
│   ├── setup/
│   │   ├── Tools Setup.md
│   │   └── content/
│   │       ├── mxpy-install-upgrade.md
│   │       ├── sc-meta-install-upgrade.md
│   │       ├── ...
│   ...     ...
│
├── networks/
│   ├── Networks & Endpoints.md
│   └── content/
│       ├── api-endpoints.md
│       ...
│
├── dapps/...
├── smart-contracts/...
├── sdks/...
├── templates/...
...
```

## Usage

When executing a specific task, one or multiple table of contents files can be included in the AI context. This allows for building a token efficient context of available topics and topic subjects, enabling the AI model to quickly understand what information is available, and where to find more details.

Detailed information linked to files in the content subdirectory, can includes extensive specifications, usage guides, code examples, etc.

>[!NOTE]
>AI agents can access detailed instructions in content files on demand, based on the table of contents files, their current task and required information, using their own intelligence and built-in tools, creating their own context.

## xPilot Integration

xPilot automatically retrieves the contents of this repository using the `/Git Instructions` command. Table of contents files related to current tasks can be quickly activated into context from the Instructions menu, to provide an overview of available information. Detailed content files are accessed on demand.

## Contribution

This library is open to anyone for contributing and expanding on any topics.