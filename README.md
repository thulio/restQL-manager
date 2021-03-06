# restQL Manager

This projects provides a Web UI over the restQL Admin API in order to facilitate daily operations like query creation, resource mappings, debugging and experimentation.

restQL Manager requires an [restQL](https://github.com/b2wdigital/restQL-golang) instance with the Admin API enabled.

## Building

The build will produce a directory with static files that can be served from a object storage like AWS S3 or, more traditionally, with an Nginx or Expresse server.

The restQL Manager depends on one environment variable, `REACT_APP_RESTQL_URL`. Hence, the command to built it must be like this:

```bash
REACT_APP_RESTQL_URL=http://my-restql.corp/ npm run build
```

## Developing

```
REACT_APP_RESTQL_URL=http://my-restql.corp/ npm start
```
