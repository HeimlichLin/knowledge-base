# GitHub Copilot Instructions for Knowledge Base

This repository is a Jekyll-based personal knowledge base hosted on GitHub Pages.

## Architecture & Structure
- **Framework**: Jekyll (Static Site Generator).
- **Theme**: `jekyll-theme-minimal`.
- **Root**: `d:\JAVA_WORKSPACE\Document`.
- **Content**: Located in `notes/<category>/`.
- **Configuration**: `_config.yml` defines `baseurl: "/knowledge-base"`.

## File Creation Standards
When creating new notes (Markdown files):
1. **Location**: Place in the appropriate subdirectory under `notes/` (e.g., `notes/programming/`, `notes/tools/`).
2. **Front Matter**: ALWAYS include YAML front matter at the top of the file:
   ```yaml
   ---
   layout: default
   title: <Descriptive Title>
   ---
   ```
3. **Language**: Use Traditional Chinese (zh-TW) for content unless otherwise specified.
4. **Formatting**: Use standard GFM (GitHub Flavored Markdown).

## Navigation & Linking
- **Manual Indexing**: There is no auto-generated sidebar. You MUST manually update the `index.md` of the parent directory when adding a new file.
- **Link Format**: Use relative paths.
  - Example: In `notes/tools/index.md`, link to `git-basics.md` as `- [Git 基本指令](git-basics.md)`.
- **Back Links**: Include a "Back to Home" or "Back to Parent" link at the bottom of index files if appropriate, e.g., `[← 返回首頁](../../)`.

## Development Workflow
- **Local Preview**:
  ```bash
  bundle exec jekyll serve
  ```
  Access at `http://localhost:4000/knowledge-base/`.
- **Dependencies**: Managed via `Gemfile`.

## Key Files
- `_config.yml`: Main configuration.
- `notes/**/index.md`: Category index files acting as navigation menus.
- `README.md`: Project documentation.
