# Lab 07 — Nova Responsive Website

A beginner-friendly, responsive multi-section website created for the Lab 07 requirements.

## Included regions
- Navigation bar with mobile menu
- Hero section with call-to-action
- Three-card feature grid
- Contact form and footer

## Run locally
No build tools are required. Open `index.html` in a browser, or use the VS Code Live Server extension.

## Responsive checks
The stylesheet includes mobile-first refinements for:
- Mobile: 375px
- Tablet: 768px
- Desktop: 1440px

Use browser DevTools responsive mode and check each viewport for horizontal overflow.

## Figma MCP configuration
The `.vscode/mcp.json` file contains the remote Figma MCP endpoint. In VS Code, open the Command Palette and follow the MCP server setup/authentication prompts. Availability and exact UI can vary by IDE version.

## Figma design handoff
This package is the working website source; it does not create or publish a Figma cloud file. To make the required editable Figma deliverable:
1. Create a new Figma Design file and a Desktop frame (1440px wide).
2. Rebuild the four regions from the website using Auto Layout (Shift+A).
3. Use the semantic layer names listed in `FIGMA_HANDOFF.md`.
4. Create the color and spacing variables listed there.
5. Add Tablet (768px) and Mobile (375px) frames and adjust the card grid to stack.
6. Share the file with **Anyone with the link — can view**, then copy the file URL.

## GitHub + deployment
1. Create a public GitHub repository.
2. Upload all files in this folder (including `.vscode/mcp.json`).
3. For GitHub Pages: repository Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save.
4. Wait for the Pages build to finish; the live URL will be shown in Settings → Pages.

The contact form is front-end demonstration only. It validates fields and displays a confirmation message, but does not send email or store submissions until connected to a backend/form service.
