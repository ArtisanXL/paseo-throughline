# paseo-throughline

A [Paseo](https://paseo.sh) plugin. See [OVERVIEW.md](OVERVIEW.md) for what it does and the [plugin docs](https://paseo.sh/docs/plugins) for the plugin model.

## Install

```bash
paseo plugin install github:ArtisanXL/paseo-throughline
```

Plugins are trusted, unsandboxed code and must be enabled on the daemon first (Settings > Plugins).

## Development

```bash
npm install
npm run typecheck
paseo plugin install "$(pwd)"
paseo plugin reload paseo-throughline
paseo plugin logs paseo-throughline
```

Layout: `index.client.tsx` and `client/` run in the app, `index.server.ts` and `server/` run in the daemon subprocess, `shared/` is imported by both.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Report vulnerabilities as described in [SECURITY.md](SECURITY.md).

## License

[MIT](LICENSE)
