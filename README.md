# Manage your CV more effectively.

- Write your CV and generate it in YAML in a single command, and (help) remove the headache that comes with having multiple drafts written in Word in a folder on your desktop.

## Installing

To run this, you will need Docker, Docker Compose, and Taskfile installed:

Docker          - [Install](https://docs.docker.com/desktop/)
Docker Compose  - [Install](https://docs.docker.com/compose/install/)
Taskfile        - [Install](https://taskfile.dev/docs/installation)

## Build your CV

- To create a new, blank resume template, use:

```sh
task create_new_blank_resume NAME="John Doe"
```

- To refresh and re-build your resume after you've made some changes, use:

```sh
task build RESUME="./John_Doe_CV.yaml"  # or to whichever YAML file you want to use
```

I also recommend reading the [RenderCV docs](https://docs.rendercv.com/developer_guide/documentation/) - they are pretty neat!

That's about it. I also suggest maybe setting up a git hook on every commit, 
just so that you are sure you have the most up-to-date version in your rendercv_output
folder. But that's just how I've gone about doing it. 
