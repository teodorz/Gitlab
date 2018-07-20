# Docker Compose defintion for spinning up Gitlab

This repository contains a docker compose definition for spinning up Gitlab using the latest official docker image of Gitlab Comunity Edition.

To abide by the best practices, the database (PostgreSQL) and messaging queue (Redis) applications have been split into 2 seperate docker containers from the Gitlab container.

These containers all use the official docker images.

Furthermore the docker compose definition provided includes integration with LDAP. Please note that for the docker image of Gitlab Community Edition, you can only use the LDAP user credentials for your permission model since the LDAP groups are available only in the Enterprise Edition.

NOTE: You can use this setup on its own or you can include it in your Accenture DevOps Platform (ADOP) setup, as long as in both cases you have an LDAP server configured.
To use together with your ADOP setup you can include the docker-compose definition provided into the ADOP one which you can find followin the next link: https://github.com/Accenture/adop-docker-compose

