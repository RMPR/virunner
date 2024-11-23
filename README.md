# Virunner

The idea is to create a visudo like experience for Github self-hosted runners.
The web UI sucks. The goal is to create a TUI that has the same view as ranger.
With the agents being the top-level folders, the runners being the subdirectories
and the labels being the files.

# TODO

- [ ] Fetch the endpoint for the runners
curl -L \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR-TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/orgs/ORG/actions/runners

- [ ] Convert it to a tree data structure

- [ ] Display the agents in the left pane

- [ ] Display the runners in the middle pane

- [ ] Display the labels in the right pane

- [ ] Allow changing the status of the agent

- [ ] Allow changing the status of the runner

- [ ] Allow changing the status of the label

- [ ] Add autocompletion for the labels
