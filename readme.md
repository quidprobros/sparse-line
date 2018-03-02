What is?
===
`sparseline` is a low resource alternative to the powerline options out there. What this means is that it only makes subtle augmentations to your prompt with a focus on git repos.


`sparseline` is written with `bash` in mind.


features
===
* this is prefixed to PS1: `« remote/branch#short_hash »`

The "short_hash" is replaced with local tag when applicable.

Example: `« origin/master#77f6ff4 » • 19:02:57|ramos@Prometheus:[sparse-line]>`


usage
===
Simple source the file from the appropriate bash config file:
```bash
source /path/to/sparseline
```


critique
===
* osse@freenode#git: I think it might be a bit naïve. For example the file refs/heads/somebranch doesn't necessarily exist even when the branch does
* lupine@freenode#git: some refs are stored in `.git/packed-refs` and so grepping `refs/*` is not enough; Not sure actually, it makes sense that local branches aren't packed that way
* _ikke_ git gc will pack local branches
