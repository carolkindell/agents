# agents

Use the tools as database such as Google Drive, email, GitHub, Notion, local folder on pc, etc...

The agents should be able to run only in the serveless backend, oberve specific folders or paths, have schedulers to execute tasks, and so on.

# example

The agent observes a folder on Google Drive, there is a root file with the prompt and context about what tasks the agents could do in the folder.
Then the agent can be configurated from that file and starts running from there. No UI needed.

# root file structure (rfs)

The rfs is a json for easy parsing in the backend.

```
{
  prompt: "text used to give commands to the agent",
  description: "short description of the task/s for human understanding",
  name: "name your agent",
  scheduler: "10s", // the time the scheduler will observe the folder (optional),
  context: "information that is needed to complete the task/s",
  ...?
}
```
