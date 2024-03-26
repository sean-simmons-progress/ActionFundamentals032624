# general notes

## webhooks
- Trigger
    - webhook
    - scheduled
    - manual
    - starter.yml

## jobs and steps
- Map - run in parallel
- can be chanined using `needs` keyword
- runs on a runner in one process
- contains a sequence of steps
- steps can be a shell command (run) or an action (uses)

## actions
    - reusable step 
    - Lives in a git repo
    - synatx:
        ```
        {owner}/{repo}@{ref}
        {owner}/{repo}/{path}@{ref}
        ./.github/actions/my-action
        ```
    - pass vars to action:
        - `with:`
        - `env:`

### docker action
    - run a docker container as an action