Easily author and add Parameterized Executors to the src/executors directory.

Each YAML file within this directory will be treated as an orb executor, with a name which matches its filename.

Executors can be used to parameterize the same environment across many jobs. Orbs nor jobs require executors, but may be helpful in some cases, such as: parameterizing the Node version for a testing job so that matrix testing may be used.

View the included hello.yml example.

description: >
  This is a sample executor using Docker and Node.
docker:
  - image: 'cimg/node:<<parameters.tag>>'
parameters:
  tag:
    default: lts
    description: >
      Pick a specific circleci/node image variant:
      https://hub.docker.com/r/cimg/node/tags
    type: string



See:

    Orb Author Intro
    How To Author Executors
    Node Orb Executor
