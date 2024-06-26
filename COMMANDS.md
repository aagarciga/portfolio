# Command History

## Project creation

This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

```bash
npx create-next-app@latest
```

## Configuring github

```bash
 git remote add origin https://github.com/aagarciga/portfolio.git
 git branch -M main
 git push -u origin main
```

## Storybook for Next.js

```bash
npx storybook@latest init
```

## FAQ

### Versioning untracked files

Due to changing letter case of a folder or file in components folder. The cache didn't track it, meaning it ws pushing the old version.

This can be fixed by doing:

```bash
git rm -r --cached .
git add --all .
git commit -a -m "Versioning untracked files"
git push origin main
```

To avoid same issue in future commits do:

```bash
git config core.ignorecase false
```

wich will then show files with changes cases for you to re-commit.
