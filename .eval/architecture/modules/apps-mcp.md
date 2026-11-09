# Module: apps/mcp

A Model Context Protocol (MCP) server that provides stdio-based tool integrations for AI/LLM clients to interact with the Karakeep API to manage bookmarks, search (FTS, semantic, and hybrid), lists, highlights, tags, and assets.

## Key files
- `apps/mcp/src/index.ts`: CLI entry point initializing and serving the MCP server over stdio
- `apps/mcp/src/shared.ts`: Shared setup creating the Karakeep API SDK client, tool registration registry, Turndown service, and MCP server factory
- `apps/mcp/src/bookmarks.ts`: Registers and implements MCP tools for searching, retrieving, creating, updating, and deleting bookmarks
- `apps/mcp/src/highlights.ts`: Registers and implements MCP tools for listing, fetching, creating, updating, and deleting bookmark text highlights
- `apps/mcp/src/lists.ts`: Registers and implements MCP tools for bookmark lists and list memberships
- `apps/mcp/src/tags.ts`: Registers and implements MCP tools for tag management and attaching/detaching tags on bookmarks
- `apps/mcp/src/assets.ts`: Registers and implements MCP tool for retrieving temporary signed URLs for downloading assets
- `apps/mcp/src/utils.ts`: Formatting and compacting helpers for serializing API objects into textual tool response representations and error handling

## Public interface
- stdio transport via serveStdio in apps/mcp/src/index.ts
- MCP Tool: get-asset
- MCP Tool: search-bookmarks
- MCP Tool: get-bookmark
- MCP Tool: get-bookmark-lists
- MCP Tool: create-bookmark
- MCP Tool: update-bookmark
- MCP Tool: list-highlights
- MCP Tool: get-bookmark-highlights
- MCP Tool: get-highlight
- MCP Tool: create-highlight
- MCP Tool: update-highlight
- MCP Tool: delete-highlight
- MCP Tool: get-lists
- MCP Tool: get-list
- MCP Tool: update-list
- MCP Tool: delete-list
- MCP Tool: add-bookmark-to-list
- MCP Tool: remove-bookmark-from-list
- MCP Tool: get-list-bookmarks
- MCP Tool: attach-tag-to-bookmark
- MCP Tool: detach-tag-from-bookmark
- MCP Tool: get-tags
- MCP Tool: get-tag
- MCP Tool: update-tag
- MCP Tool: delete-tag
- MCP Tool: get-tag-bookmarks

## Dependencies
- @modelcontextprotocol/server
- @karakeep/sdk
- @karakeep/shared
- zod
- turndown
- vite
- vitest

## AI touchpoints [AI]
- `apps/mcp/src/index.ts`
- `apps/mcp/src/bookmarks.ts`
- `apps/mcp/src/highlights.ts`
- `apps/mcp/src/lists.ts`
- `apps/mcp/src/tags.ts`

## Open questions
- _none_
