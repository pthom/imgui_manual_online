Website for https://pthom.github.io/imgui_manual_online/

This is a minimal static site that hosts the [ImGui Manual](https://github.com/pthom/imgui_manual).

## Structure

- `index.html` - Root page that redirects to the manual
- `manual/` - Contains the ImGui Manual built with emscripten
  - `imgui_manual.html` - The main manual application
  - `imgui_manual.js`, `imgui_manual.wasm`, `imgui_manual.data` - WebAssembly files
  - `imgui_manual_favicon.png` - Favicon

## Deployment

The manual is automatically deployed using the `tools/deploy_imgui_manual.sh` script in the parent repository.

GitHub Pages serves the site from the root directory.

## Building

To build and deploy:

1. Build the manual: `./tools/emscripten_build.sh` (from parent repo)
2. Deploy: `./tools/deploy_imgui_manual.sh` (from parent repo)
