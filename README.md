# Boilerplate project

- Uses [T3 Stack](https://create.t3.gg/) project bootstrapped with `create-t3-app`.
- Uses Docker & Docker Compose to run

## How to run

- Make sure Docker & Docker Compose are installed
- Run `docker-compose up -d`
- Run migrations: `docker-compose run app yarn prisma:migrate:dev`
- The app should be up and running at http://localhost:3000

## Command Line utility

You can use the command line utility to issue commands that will run on containers.

The utility is setup at `misc/dev-tools/bin/pf-dev`. To make it easier to use it, you can add the `misc/dev-tools/bin` folder to your path. Just put this on `.bash_profile` or `.bashrc`:

```bash
export PF_DIR="$HOME/path/to/project" # You should use the path the project is located at your machine
export PATH="$PF_DIR/misc/dev-tools/bin:$PATH"
```

Now you can use like this:

```bash
pf-dev start
pf-dev stop
```

You can check `pf-dev help` and see how to use it
