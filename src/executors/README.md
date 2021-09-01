Easily author and add Parameterized Executors to the src/executors directory.

Each YAML file within this directory will be treated as an orb executor, with a name which matches its filename.

Executors can be used to parameterize the same environment across many jobs. Orbs nor jobs require executors, but may be helpful in some cases, such as: parameterizing the Node version for a testing job so that matrix testing may be used.

View the included hello.yml example.

See:

    Orb Author Intro
    How To Author Executors
    Node Orb Executor
