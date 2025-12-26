# GitHub Pages Deployment Guide

## Configuration Summary

This repository has been configured for deployment to GitHub Pages at:
**https://UCUmovenglab.github.io/ucumovenglab/**

## Changes Made

1. **Updated `_config.yml`:**
   - Set `baseurl: "/ucumovenglab"` (required for project sites)
   - Set `url: "https://UCUmovenglab.github.io"`

2. **Fixed internal links in `index.md`:**
   - Updated links to use `{{ site.baseurl }}` for proper URL generation

3. **GitHub Actions workflow:**
   - Already configured in `.github/workflows/jekyll.yml`
   - Automatically builds and deploys on push to `main` branch

## Enabling GitHub Pages

To enable GitHub Pages for this repository:

1. Go to the repository settings: https://github.com/UCUmovenglab/ucumovenglab/settings/pages
2. Under "Build and deployment":
   - Source: Select "GitHub Actions"
3. Save the settings

Once enabled, the site will be automatically deployed whenever changes are pushed to the `main` branch.

## Verifying Deployment

After merging to `main` and enabling GitHub Pages:

1. Check the Actions tab for deployment status: https://github.com/UCUmovenglab/ucumovenglab/actions
2. Once the workflow completes, visit: https://UCUmovenglab.github.io/ucumovenglab/

## Local Development

To run the site locally:

```bash
bundle install
bundle exec jekyll serve
```

Then visit: http://localhost:4000/ucumovenglab/

## Alternative: Organization Site

If you want the site to be available at `https://UCUmovenglab.github.io` (without the `/ucumovenglab` path):

1. Rename this repository to `UCUmovenglab.github.io`
2. Update `_config.yml`:
   - Change `baseurl: ""` (empty string)
   - Keep `url: "https://UCUmovenglab.github.io"`
3. Update internal links to remove `{{ site.baseurl }}` or keep them (they'll work with empty baseurl)

This would make the site the organization's main GitHub Pages site.
