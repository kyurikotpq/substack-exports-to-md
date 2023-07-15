# Convert Substack Posts into Markdown Files

## Functionality
This Jupyter Notebook takes a Substack export (in the format as of June 2023) and converts the HTML posts into Markdown files.

## Use Case
I would like to create an archive of posts in Gatsby (where I'll be hosting my personal website). To achieve this, I need the post in Markdown files.

## Folder Structure

```
/root
├── converter.ipynb
├── posts.csv         # From Substack Imports
├── converted-posts/  # CREATED AUTOMATICALLY - tracked in OUTPUT_FOLDER
├── img/              # CREATED AUTOMATICALLY
├── posts/            # From Substack Imports — tracked in INPUT_FOLDER
│   ├── post-1.html
│   ├── post-1.delivers.csv
│   ├── post-1.opens.csv
|   ├── ... (other posts)
```

## Caveats
- I haven't escaped titles from special characters like `:`, which would mess up the YAML frontmatter.
- You'll have to resolve links to Substack posts and embeds manually
