# Project Guidelines

## Development Workflow
1.  **Local Testing**: Always run `bundle exec jekyll serve` and verify changes at `http://localhost:4000` before committing.
2.  **Post Creation**: New posts should be added to the `_posts/` directory following the `YYYY-MM-DD-title.md` format.
3.  **Configuration**: Changes to `_config.yml` require a restart of the Jekyll server to take effect.

## Content Standards
- Use Markdown for all posts and pages.
- Ensure front matter (the YAML at the top of files) is correctly formatted.
- Descriptive titles and categories should be used where applicable.

## Dependency Management
- Use `bundle install` to synchronize gems.
- Avoid manual edits to `Gemfile.lock`.
- Link to official [Jekyll Documentation](https://jekyllrb.com/docs/) when introducing new features or plugins.
