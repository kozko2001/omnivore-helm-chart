# omnivore-helm-chart

## Values

```
postgres.enabled: true    # if you want to create a postgres service
postgres.user: postgres   # username for the database
postgres:password: postgres # password for the database
postgres:dbName: omnivore # database name
postgres.pgPoolMax: 20    # ??? it's in the docker-compose of omnivore
postgres.persistence.enabled: true   # to manage persistence in the chart
postgres.size: 8Gi        # Size for the database

elasticsearch.enabled: true    # if you want to create a postgres service
elasticsearch.persistence.enabled: true   # to manage persistence in the chart
elasticsearch.size: 8Gi        # Size for the database

```

## Development

- `helm lint`: check the linting of the chart
- `helm install omnivore-release .  --namespace omnivore`: to tryout the version you have in development
- `helm template omnivore-release .`: to see what will generate in case of error


