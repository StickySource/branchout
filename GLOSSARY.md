# Terms and Variables Defined

## Terms defined and orhan terms

- `BRANCHOUT_NAME` - The common name for both the meta project directory and cache/settings directory for a given project.
- `BRANCHOUT_FILE` - The file name in the meta repo with the basic setup of the project tree, such as the above. Can be called either `Branchoutfile` or `.branchout`.
- `BRANCHOUT_PROJECTS` - The file name in the meta repo where the project names are listed in raw form with prefix (if any) and group. Can be called either `Branchoutprojects` or `.projects`.
- `BRANCHOUT_STATE` ? - **TODO** This one is the settings/cache dir specific to current meta project? Is the name appropriate? To me state of a set of repos is git status run across all of them, not maven settings and repo cache.
- `PROJECTION_DIRECTORY` ? - **TODO** This one stands out like a sore thumb - rename to `BRANCHOUT_PROJECTION_DIR`?
- `BRANCHOUT_PROJECTS_DIRECTORY` ? - **TODO** sub directory under home under which branchout meta projects live - needs to be independent of ${HOME}
- `BRANCHOUT_STATES_DIRECTORY` ? - **TODO** doesn't yet exist, equivalent to the above, but for the settings/caches directory structure for each meta project.
- `BRANCHOUT_GIT_BASEURL` - The prefix for all git repos included in a particular branchout meta project. Derived, but can be overriden in case the base project differs from the rest (unlikely).
- `BRANCHOUT_PATH` - The path under which the `branchout` script lives and under which it knows it can find its siblings in order to explicitly call them rather than relying on them being on the path (which breaks if the script is called with a direct call and isn't on the path).

## Definitions needing a home above

1. The root directory where branchout meta projects live side by side with each other. Where the branchout init process places new meta projects in folders called `BRANCHOUT_NAME`.
2. The root directory where branchout places project-specific folders called `${BRANCHOUT_NAME}` side by side with settings and cache directories for different tooling nested beneath.
3. ?
4. ?
5. ?


