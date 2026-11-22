---
name: create-starter
description: Create starter documentation using this plugin's bundled template. Use when asked to create a project starter document.
---

# Create a starter document

1. Read [the bundled template](templates/start-here.md). Resolve this path
   relative to this SKILL.md file, not the user's workspace.
   If the template cannot be read, report that and stop; do not invent it.
2. Read the user's project-brief.md. If it is missing, ask for it.
3. Call microsoft_docs_search on the mslearn MCP server with the public query
   "Azure Functions HTTP trigger overview". Do not send the project brief,
   local paths, or other workspace content to the server.
   If the tool fails or returns no relevant documentation, report that and stop.
4. Create PLUGIN-TEMPLATE.md in the user's workspace as an exact, unchanged
   text copy of the bundled template, including its final newline.
5. Create START-HERE.md in the user's workspace using the template's headings.
   Fill in the project name and purpose from the brief. Under Documentation,
   add a short explanation and one relevant official Microsoft Learn link
   from the tool result. Preserve the template's origin footer.
6. Report the installed template path you actually read, the MCP tool used,
   and the two files created. Do not claim a path or tool call you did not use.

If either output file already exists, ask before replacing it.
Do not change other files, run commands, build an app, or deploy anything.