# PLAYWRIGHT MCP EXECUTION PROTOCOL

1. Always call `browser_navigate` before attempting snapshots or screenshots.
2. Prefer `browser_snapshot` (accessibility tree) for text and data extraction to minimize token overhead. Reserve `browser_take_screenshot` for visual verification in Phase 4.
3. If an external site blocks content with a cookie banner or login prompt, use `browser_click` on dismiss/close elements before extracting data.