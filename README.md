# Civic Transparency CWE Types

[![Docs](https://img.shields.io/badge/docs-mkdocs--material-blue)](https://civic-interconnect.github.io/civic-transparency-cwe-types/)
[![PyPI](https://img.shields.io/pypi/v/civic-transparency-cwe-types.svg)](https://pypi.org/project/civic-transparency-cwe-types/)
[![Python 3.12+](https://img.shields.io/badge/python-3.12%2B-blue?logo=python)](#)
[![CI Status](https://github.com/civic-interconnect/civic-transparency-cwe-types/actions/workflows/ci.yml/badge.svg)](https://github.com/civic-interconnect/civic-transparency-cwe-types/actions/workflows/ci.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)

> **Typed Python models (Pydantic v2) for the Civic Transparency schema.**

> Maintained by [**Civic Interconnect**](https://github.com/civic-interconnect).
>
> - **Documentation:** https://civic-interconnect.github.io/civic-transparency-cwe-types/
- **Contributing:** [CONTRIBUTING.md](./CONTRIBUTING.md)

---

## Overview

This package provides strongly-typed Python models for the CWE Catalog transparency ecosystem.
The types are automatically generated from canonical JSON Schema definitions, ensuring consistency and validation at runtime.

**Key Features:**
- **Type Safety:** Full Pydantic v2 validation with IDE support
- **Schema Compliance:** Generated directly from official JSON schemas
- **Privacy-First:** Designed for aggregated, non-PII data exchange
- **Interoperability:** JSON serialization/deserialization with validation

## Installation

```bash
pip install civic-transparency-cwe-types
```

For development:
```bash
pip install "civic-transparency-cwe-types[dev]"
```



---

## Quick Start

```bash
uv venv
uv pip install -e ".[dev,docs]" --upgrade
uv run ruff check . --fix && uv run ruff format .
git add -A
uv run pre-commit run --all-files
uv run -m pytest -q
uv run -m build
uv run -m mkdocs build
uv run -m mkdocs serve
```

## If Pre-Commit Issues

```
git add .
git commit -m "msg" --no-verify
git push
```

## Publish

```
uv run -m build

uv run -m mkdocs serve
uv run -m mkdocs build
```



---

## Development and Contributing

### For Type Users
- Report type-related issues here
- Request documentation improvements


### Local Development
```bash
git clone https://github.com/civic-interconnect/civic-transparency-cwe-types
cd civic-transparency-cwe-types
uv venv
uv pip install -e ".[dev,docs]"
```

See [CONTRIBUTING.md](./CONTRIBUTING.md) for detailed guidelines.

---

## Support and Community

- **Documentation:** https://civic-interconnect.github.io/civic-transparency-cwe-types/
- **Issues:** [GitHub Issues](https://github.com/civic-interconnect/civic-transparency-cwe-types/issues)
- **Discussions:** [GitHub Discussions](https://github.com/civic-interconnect/civic-transparency-cwe-types/discussions)
- **Email:** info@civicinterconnect.org

---

## About Civic Transparency

Civic Transparency is an open standard for privacy-preserving, non-partisan analysis of how information spreads in civic contexts. The specification enables researchers, platforms, and civic organizations to share insights while protecting individual privacy.

**Core Principles:**
- **Privacy by Design:** No personally identifiable information
- **Aggregation First:** Time-bucketed, statistical summaries
- **Open Standard:** Collaborative, transparent development
- **Practical Implementation:** Real-world deployment focus
