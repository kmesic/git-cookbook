# Git Cookbook

This is cookbook for a cheatsheet of various git workflows and commands. It's also a place where you can learn how git really works.

Visit the cookbook at: https://kmesic.github.io/git-cookbook/

If you want to contribute to the project, then you are at the right place!

## Background

Git is sometimes scary for people, but if you truly understand its design, then your productivity can tremoudously increase. Along with that you can finally understand the true power behind it.

Also sometimes you just don't want to think about what commands to run. This is your place where you can find various workflows of git commands. And then just copy and paste into your terminal :simple_smile:

This project was built with [mdbook](https://github.com/rust-lang/mdBook)

## How to contribute

I encourage all contributions! :rocket::rocket::rocket:

1. Decide if you plan on making a large contribution or a small one (read below if confused)
2. If large contribution, file an issue
3. Fork the repo

### Github Editor (Easiest)

The easiest way to contribute, is to edit the files right in Github and commit them. 

A CI task will generate the JS, HTML files required for the website. 

All the markdown files are located in [src](src).

### Local Development (Hardest)
1. Install Rust and Cargo
2. Install mdbook via Cargo
```
cargo install mdbook
```
3. Read [mdbook](https://github.com/rust-lang/mdBook) to run commands
4. Basic commands:
```
---Build (Generate HTML/JS/CSS files)---
mdbook build

---Serve the site on http://localhost:3000---
mdbook serve
```

No need to check in the generated HTML/JS/CSS files. All are generated as part of a CI task on every pull request.

.gitignore should ignore them in the first place.

### Large Contribution
Please first file an issue, and wait till I comment to go ahead and take up the work.

Examples of a large contribution:
- New page
- New section
- Major rewrite of a section

### Small Contribution
However, for small contributions, no need to create an issue and wait for approval. Feel free to send over the pull request. 

Examples of a small contribution:
- Grammatical change
- Typo fix
- Reword of a sentence

