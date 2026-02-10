# Meet Satoshi - meetsatoshi.org

## Project Goal

Build a comprehensive archive website at **meetsatoshi.org** to collect, organize, and present all publicly available content from Craig Steven Wright (CSW), including but not limited to:

- Blog posts (craigwright.net, etc.)
- Twitter/X posts
- YouTube videos and recorded talks
- Interviews (text, audio, video)
- Conference presentations and meeting transcripts
- LinkedIn posts and articles
- Court documents and testimonies
- Academic papers and publications
- Slack/forum discussions

The goal is to create a searchable, well-organized public resource for anyone researching CSW's public statements and writings.

## Tech Stack

- **Static Site Generator**: Hugo
- **Theme**: Ananke (via git submodule)
- **Hosting**: Cloudflare Pages
- **Domain**: meetsatoshi.org (registered via name.com)
- **Source Control**: GitHub

## Project Structure

```
content/
  _index.md          # Homepage
  blog/              # Blog post archives
  tweets/            # Twitter/X posts
  videos/            # Video content (YouTube, etc.)
  interviews/        # Interviews
  conferences/       # Conference talks and presentations
  papers/            # Academic papers and publications
  about/             # About this project
```

## Development

```bash
# Run local dev server
hugo server -D

# Build for production
hugo --minify
```

## Deployment

- Push to `main` branch on GitHub triggers Cloudflare Pages build
- Build command: `hugo --minify`
- Build output directory: `public`
