## Development

```
./run && open http://localhost:8080
```

### GraphQL

GraphiQL:

```
open http://localhost:8081/graphiql
```

### Database

Create new migration:

```
./run db:migration migrationName
```

Migrate:

```
./run db:up
```

## Deployment

## Production

### Provisioning

1. Create Droplet in Digital Ocean (Ubuntu / Starter / \$5 plan)
1. Create `.env.production` file with config for production. See `.env.production.example` as a template.
1. Update the `HOST_NAME` variable to contain the droplet IP address.
1. Finally, run the following to make some config changes and install Docker on the droplet:

```
 ./run provision --prod
```

### Deploy

```
./run deploy --prod
```
