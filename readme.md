0;95;0cWhat is?
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
