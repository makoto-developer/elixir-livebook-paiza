# Elixir Livebook for Paiza

# Motivation

I wanted to be able to solve paiza(https://paiza.jp/) by Elixir, and show result running in a local device.

# Requirement

- docker
- asdf

# Getting Start

Clone this repository.

```shell
git clone git@github.com:makoto-developer/elixir-livebook-paiza.git
```

create `.env` file

```shell
cp .env.example .env


# edit secret, port, other configs, if you need.
vi .env

# edit docker-compose.yml, if you need password when livebook starting auth.
vi docker-compose.yml
# - LIVEBOOK_TOKEN_ENABLED=true

# remove comment out if you need auth.
- #- LIVEBOOK_PASSWORD=${LIVEBOOK_PASSWORD}
```

Start docker compose.

```shell
dockcer compose up -d
```

Finish docker compose if you finish work.

```shell
dockcer compose stop
```

You start livevook next time.

```shell
docker compose start
```

# Livebook

1. When you want solve paiza problem, First of all, open paiza template book.

![open_template.png](assets/open_template.png)

2. select `paiza_template.livemd`

![select_paiza_templete_livebook.png](assets/select_paiza_templete_livebook.png)

3. fork paiza

![paiza_template_fork.png](assets/paiza_tempalte_fork.png)

4. Rename livebook name.

![rename_livebook.png](assets/rename_livebook.png)

# References

- https://livebook.dev/
