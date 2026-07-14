# 🚀 aidatacooper (DataCooper AI Lab)

Welcome to **aidatacooper** — the open-source engineering lab founded by **[Cooper Wenhua](https://github.com/imgwho)**. 

Our mission is to **make Business Intelligence programmable, agent-friendly, and reproducible**. We bridge the gap between LLMs, Model Context Protocol (MCP), and Tableau to transition BI workflows from manual, error-prone drag-and-drop tasks into inspectable and safe code-first systems.

---

## 📖 The datacooper Story: Why Programmable BI?

For years, Business Intelligence has been locked behind graphical user interfaces (GUIs). While great for visual exploration, this drag-and-drop paradigm introduces major challenges for modern software teams:
*   **No Version Control**: `.twb` and `.tfl` files are XML/JSON monoliths that are difficult to diff, track, or merge in Git.
*   **Agent Barriers**: AI agents cannot easily click through desktop menus to build charts or map calculations.
*   **Lack of Validation**: There are few automated ways to ensure a workbook calculation doesn't break when a schema changes.

**datacooper** was born to solve this. We build PyPI packages, CLI compilers, and MCP servers that treat Tableau workbooks and Prep flows as **reproducible analytics assets**.

---

## 🛠️ Our Open-Source Ecosystem

We build and maintain the core engines that turn manual BI steps into programmable systems:

<p align="center">
  <img src="https://img.shields.io/badge/cwtwb-Workbook%20Engineering-E97627?style=for-the-badge&logo=tableau&logoColor=white" />
  <img src="https://img.shields.io/badge/cwprep-PrepFlow%20Automation-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/MCP-Agent%20Bridges-7C3AED?style=for-the-badge&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/cwtwb.com-Docs%20%26%20Spec-111111?style=for-the-badge&logo=githubpages&logoColor=white" />
</p>

### Featured Repositories

| Project | Target | The Core Innovation |
|---|---|---|
| 📊 **[cwtwb](https://github.com/imgwho/cwtwb)** | Tableau Workbook (`.twb` / `.twbx`) | Text-to-Workbook compiler and parser. Allows AI agents (via MCP) to dynamically edit worksheets, manage calculated fields, and validate schemas without GUI interaction. |
| 🔀 **[cwprep](https://github.com/imgwho/cwprep)** | Tableau Prep Flow (`.tfl`) | Text-to-PrepFlow engine. Translates natural language data-cleaning requests into valid Tableau Prep flows, offering offline validation, schema checking, and automated ETL staging. |

---

## 🔌 The MCP Paradigm (Model Context Protocol)

We believe AI agents should have native tools to inspect and edit your BI layer. Both `cwtwb` and `cwprep` expose standardized **Model Context Protocol (MCP)** endpoints, turning local Tableau files into contexts that LLMs (like Claude and OpenAI apps) can reason about, refactor, and build.

```json
// Hook datacooper tools directly into Claude Desktop or Cursor:
{
  "mcpServers": {
    "cwtwb": {
      "command": "python",
      "args": ["-m", "cwtwb.mcp_server"]
    },
    "cwprep": {
      "command": "python",
      "args": ["-m", "cwprep.mcp_server"]
    }
  }
}
```

---

## 🔮 The Stack We Stand On

<p>
  <img src="https://img.shields.io/badge/Claude-MCP%20Orchestration-000000?style=flat-square&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenAI-Agentic%20Products-412991?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/Tableau-Desktop%20%26%20Prep%20APIs-E97627?style=flat-square&logo=tableau&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-Automation%20SDK-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-Reproducible%20Dataops-16A34A?style=flat-square&logo=git&logoColor=white" />
</p>

---

## 💬 Connect & Collaborate

*   **Founder**: [Cooper Wenhua](https://github.com/imgwho) (AI PM focused on BI & Workflow automation)
*   **Website**: [datacooper.com](https://datacooper.com)
*   **Open Source & Issues**: Submit PRs and feedback directly on our [cwtwb](https://github.com/imgwho/cwtwb) and [cwprep](https://github.com/imgwho/cwprep) repos!
