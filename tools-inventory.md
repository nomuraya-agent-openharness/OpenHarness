# OpenHarness Tools Inventory

This document lists the tools available in the `src/openharness/tools/` directory of the OpenHarness project, describing their purpose and primary use.

## Tools List

| Tool Name | Purpose |
|---------|-------|
| `bash` | Executes shell commands in the local repository with stdout/stderr capture. Used for running system commands, scripts, and builds. |
| `read_file` | Reads the contents of a text file, optionally with line ranges. Used for inspecting source code and log files. |
| `write_file` | Creates or overwrites a text file. Used for generating or updating configuration and source files. |
| `edit_file` | Replaces a specific string in an existing file. Used for targeted updates to code and config files. |
| `glob` | Lists files matching a glob pattern, using `rg --files` when available for speed and respect of `.gitignore`. Used for finding files in the project. |
| `grep` | Searches file contents for a regular expression pattern, using `ripgrep` when available for performance. Used for code searches and log analysis. |
| `skill` | Loads a bundled, user, or plugin skill by name. Used to invoke higher-level capabilities like planning or testing. |
| `tool_search` | Searches the available tool list by name or description. Used to discover tools based on functionality. |
| `web_fetch` | Fetches a single web page and returns its content as compact, readable text after removing HTML. Used to retrieve online documentation or web content. |
| `web_search` | Performs a web search using DuckDuckGo and returns the top results with titles, URLs, and snippets. Used for researching topics or finding resources. |
| `config` | Reads or updates OpenHarness settings. Used for persistent configuration of the harness. |
| `brief` | Shortens a piece of text for compact display. Used to summarize long outputs. |
| `sleep` | Pauses execution for a specified duration. Used for delays in workflows. |
| `enter_worktree` | Creates a git worktree for a branch. Used for isolating work on feature or bugfix branches. |
| `exit_worktree` | Removes a git worktree. Used to clean up after work is complete. |
| `cron_create` | Creates or replaces a local cron job. Used for scheduling recurring tasks. |
| `cron_list` | Lists configured local cron jobs. Used to audit scheduled tasks. |
| `cron_delete` | Deletes a local cron job by name. Used to remove scheduled tasks. |
| `cron_toggle` | Enables or disables a local cron job. Used to temporarily deactivate scheduled tasks. |
| `remote_trigger` | Immediately triggers a configured local cron-style job. Used for on-demand execution of scheduled tasks. |
| `task_create` | Creates a background shell or local-agent task. Used for running long-running or asynchronous operations. |
| `task_get` | Gets details for a background task. Used for monitoring task status. |
| `task_list` | Lists background tasks. Used for task management and oversight. |
| `task_stop` | Stops a background task. Used to terminate tasks. |
| `task_output` | Reads the output log for a background task. Used to retrieve task results or logs. |
| `task_update` | Updates a task's description, progress, or status note. Used for tracking task progress. |
| `agent` | Spawns a local background agent task. Used for delegating work to sub-agents. |
| `send_message` | Sends a message to a running local agent task. Used for communicating with sub-agents. |
| `team_create` | Creates a lightweight in-memory team for agent tasks. Used for organizing multi-agent workflows. |
| `team_delete` | Deletes an in-memory team. Used for cleaning up after team-based tasks. |
| `todo_write` | Appends a TODO item to a markdown checklist file. Used for task management. |
| `enter_plan_mode` | Switches permission mode to plan, restricting actions that modify state. Used for safe planning and review. |
| `exit_plan_mode` | Switches permission mode back to default. Used to resume normal operation after planning. |
| `list_mcp_resources` | Lists MCP (Model-Context Protocol) resources from connected servers. Used for discovering available external resources. |
| `read_mcp_resource` | Reads an MCP resource by server and URI. Used to access external data or services. |
| `mcp_auth` | Configures authentication for an MCP server. Used to authenticate with external services. |
| `ask_user_question` | Asks the interactive user a follow-up question and returns the answer. Used for gathering input during interactive sessions. |
| `notebook_edit` | Creates or edits a Jupyter notebook cell. Used for interactive data science and analysis. |
| `lsp` | Inspects Python code using Language Server Protocol features like definitions, references, and symbols. Used for code navigation and understanding. |
| `sleep_tool` | Pauses execution for a short duration. (Note: likely a duplicate of `sleep`) |
