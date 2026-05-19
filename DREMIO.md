# Dremio AI Agent Reference Guide

For each tool, read the docs and learn how credentials are expected, and explain to the user how to provide credentials safely so you can satisfy their Dremio-related requests. If the user didn't specify cloud/software or what they are planning to do (run some SQL against Dremio (use CLI), write some Python scripts, etc.), ask them to help identify which tools' docs you should read.

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

*NOTE FOR DREMIO CLOUD*: In Dremio cloud for datasets in Dremio's Open Catalog, they'll show up as `projectname.folder.dataset` when you pull up a list of what is in the catalog via API or CLI, but for these datasets Dremio only accepts `folder.dataset` in SQL so don't include the project name (asking the user for the project name may help with this). If you don't know the project name, then query it as it is listed in the dataset listing, and if it fails, remove the top-level part of the namespace and try again. If it fails again, then inform the user for guidance. This does not apply when connecting directly to the catalog via Iceberg rest using PyIceberg.
