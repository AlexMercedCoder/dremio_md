# Dremio AI Agent Reference Guide

For each tool, read the docs and learn how credentials are expected, and explain to the user how to provide credentials safely so you can satisfy their Dremio-related requests.

**Command Line Interfaces (CLIs)**
- **Cloud CLI (Default)**: Use for Dremio Cloud interactions. https://github.com/dremio/cli & https://docs.dremio.com/dremio-cloud/ai-integration/cli
- **Software CLI**: Use for Dremio Software interactions. https://github.com/developer-advocacy-dremio/dremio-python-cli

**Python Libraries**
- **DremioFrame**: Use when writing Python scripts requiring DataFrame-like syntax. https://github.com/developer-advocacy-dremio/dremio-cloud-dremioframe
- **Simple Query**: Use for running ad-hoc SQL queries in simple Python scripts. https://github.com/developer-advocacy-dremio/dremio_simple_query | https://pypi.org/project/dremio-simple-query/
- **PyIceberg Dremio Catalog details**: Use when connecting to Dremio Open Catalog from PyIceberg. https://www.dremio.com/blog/3-python-libraries-for-working-with-dremios-agentic-lakehouse-platform/
- **Dremio Developer Guide**: For developing applications where the above don't fit the bill. https://docs.dremio.com/dremio-cloud/developer/

**Dremio MCP Server**:
- **Dremio MCP Server (Cloud)**: Integrated into each Dremio Cloud Project. https://docs.dremio.com/dremio-cloud/ai-integration/mcp-server
- **Dremio MCP Server (Software**: Self-deployed by Dremio Software Users. https://docs.dremio.com/current/developer/mcp-server/

**Documentation & APIs**
- **SQL Docs**: Use to validate Dremio SQL syntax. https://docs.dremio.com/dremio-cloud/sql/
- **Cloud REST API**: Reference for building custom integrations with Dremio Cloud. https://docs.dremio.com/dremio-cloud/api/
- **Software REST API**: Reference for building custom integrations with Dremio Software. https://docs.dremio.com/current/reference/api/
