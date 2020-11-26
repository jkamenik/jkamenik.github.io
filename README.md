# [jkamenik.github.io](https://jkamenik.github.io)

This is the source for my resume.

The branch `master` is the statically rendered site.  `draft` is the dymanic Jekyll site.

```bash
git clone --recurse-submodules git@github.com:jkamenik/jkamenik.github.io.git
cd jkamenik.github.io
git checkout draft
git submodule update --init
./runme
```

In the `draft` branch the `_site` directory is the `master` branch.  So after adjusting the site, you can simply commit there.

```bash
cd _site
git add ...
git commit ...
git push
```

## Site Layout

As a resume the entire site is meant to compile into a single
document, but for easy of maintenance it is split into multiple files.
These files are included in the following order:

1. Header - Name, Email, Phone, and Links
1. Summary
1. Skills
1. Open Source
1. Experience
1. Education
1. Footer - Copyright

## Print Media

A print media CSS is provided which changes the colors and fonts to
look better on the printed page.  Also, the header and footer are
hidden and links are expanded.
