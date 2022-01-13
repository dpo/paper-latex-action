# Paper

## How to Clone

1. Clone the `latex-styles` repository
    ```
    git clone https://github.com:dpo/latex-styles.git
    ```
2. Clone this repository and apply the default hooks
    ```
    git clone --template=latex-styles https://github.com:user/name_of_this_repo.git
    ```

## Create an empty branch where PDF artifacts will be published

An empty branch named `pdfs` must be pushed to the remote where PDF artifacts
generated when submitting pull requests can be pushed:

```bash
git checkout --orphan pdfs
git rm -rf .
git commit --allow-empty -m "root commit"
git push origin pdfs
```

## Conventions

1. Write clean LaTeX code:
    * write *readable* LaTeX, as you would write readable Python, Julia, Matlab, etc.
    * indent two spaces, no tabs,
    * set your text editor to wrap long lines
    * one line = one sentence
2. Use `hyperref`, `nameref` and `cleveref` whenever possible

Enjoy!
