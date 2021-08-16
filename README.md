# Code for generating my personal website

This repository contains code used to generate [my personal website](https://peterhcharlton.github.io).

## Instructions for use

I use the following instructions to modify my website.

### Edit Files

1. The _starter-hugo-academic_ repo should be visible in GitHub desktop. (I cloned it from [peterhcharlton/starter-hugo-academic](https://github.com/peterhcharlton/starter-hugo-academic)
2. Make any changes to the markdown files in the local repo: _starter-hugo-academic_

### Compile website
1. Delete the 'public' directory within the 'starter-hugo-academic' repo (if it's there).
2. Open Terminal (or command prompt)
3. Make the current directory the _starter-hugo-academic_ repo directory. _e.g._ run: `cd ~/Documents/GitHub/starter-hugo-academic`
4. To preview locally, run: `hugo server`, then navigate to: http://localhost:1313/
5. To compile the website in the 'public' folder, run: `hugo`

### Upload files

1. The _peterhcharlton.github.io_ repo should be visible in GitHub desktop (I cloned it from [here](https://github.com/peterhcharlton/peterhcharlton.github.io)).
2. Delete everything in the _peterhcharlton.github.io_ repo, apart from '.git' (which is a hidden directory).
3. Copy the contents of the 'public' folder to the 'peterhcharlton.github.io' repo, and commit.

## Helpful tips

For general instructions, see: https://wowchemy.com/docs/guide/deployment/

For instructions on authentication at the command line see: https://ginnyfahs.medium.com/github-error-authentication-failed-from-command-line-3a545bfd0ca8

If you see:
`Error: from config: failed to resolve output format "WebAppManifest" from site config`
then:
- as described [here](https://wowchemy.com/docs/guide/troubleshooting/#error-failed-to-resolve-output-format)
- temporarily remove the "WebAppManifest", "redirects", "headers" output types from your config.yaml
- run:
  ``hugo mod clean``
  ``hugo mod tidy``
- replace the "WebAppManifest", "redirects", "headers" output types in your _config.yaml_ file


## Source

The website is generated using the Academic Template for [Hugo](https://github.com/gohugoio/hugo).
