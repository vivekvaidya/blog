# Blog Maintenance Guide

This guide explains how to maintain and update your blog.

## Creating New Posts

To create a new blog post:

1. Create a new file in the `_posts` directory
2. Name it with the format: `YYYY-MM-DD-post-title.md`
3. Add the following front matter at the top:

```
---
layout: post
title: "Your Post Title"
---
```

4. Write your post content in Markdown below the front matter
5. Commit and push to GitHub to publish

## Example Post Format

```markdown
---
layout: post
title: "My New Post"
---

This is the content of my new blog post. I can use **bold text**, *italic text*, and [links](https://example.com).

## This is a heading

I can organize my content with headings.

- This is a list item
- This is another list item
```

## Updating Existing Posts

To update an existing post, simply edit the file in the `_posts` directory and commit the changes.

## Adding Images

To add images to your posts:

1. Place image files in the `public` directory
2. Reference them in your posts with:

```markdown
![Alt text](/public/image-name.jpg)
```

## Customizing the Site

### Changing Colors and Styles

Modify the variables in `_sass/_variables.scss` to change colors and fonts.

### Updating Bio Information

Update your bio information in:
- `_config.yml` - for site title and contact info
- `index.html` - for the main bio section
- `about.md` - for the detailed about page

### Adding New Pages

To add new pages:
1. Create a new `.md` file in the root directory
2. Add front matter specifying `layout: page`
3. Write your content in Markdown

## Deployment

The site is automatically deployed when you push to the `master` branch of your repository. It may take a few minutes for changes to appear.

## Troubleshooting

If your site isn't updating:
1. Check that your commits have been pushed to GitHub
2. Verify there are no build errors in the GitHub repository settings
3. Ensure your custom domain is properly configured in repository settings