# Simple docker-compose for Odoo

This docker-compose create:
- Container with Odoo 8
- Container with Postgres 9.4
- Contanier with volume for PostgreSQL
- Container with volume for Odoo (conf file and addons)

It is required to have installed [Docker] (https://docs.docker.com/compose/install/) and [Docker Compose] (https://docs.docker.com/compose/install/). Optional (windows/mac) [Docker machine] (https://docs.docker.com/machine/install-machine/).

### Instructions:

Modify the file docker_data/config/openerp-server.conf (if necessary), add the extras addons in the folder docker_data/extra_addons and run the follow command:

```sh
$ docker-compose up -d
```

And then access to <ip>:8069

To view Odoo's logs use:

```sh
$ docker logs -f odoo8
```

License
----

MIT