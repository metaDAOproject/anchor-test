# Anchor Test

A fast, easy, and secure action for testing [Anchor](https://www.anchor-lang.com/) projects. Completes in ~1 minute.

## Usage

### Example workflow

Here's an example workflow:

```yaml
name: example-workflow
on: [push]
jobs:
  run-anchor-test:
    runs-on: ubuntu-22.04
    steps:
      - uses: actions/checkout@v3
      - uses: metadaoproject/anchor-test@v2.3
```

This will use the default versions of Anchor, Node.js, and the Solana CLI tools, which are 0.27.0, 16.15.1, and 1.15.2 respectively. 

### Configuring versions

You can also configure these versions like so:

```yaml
steps:
  - uses: actions/checkout@v3
  - uses: metadaoproject/anchor-test@v2.3
    with:
      anchor-version: '0.29.0'
      solana-cli-version: '1.18.26'
      node-version: '16.15.1'
```

### Cargo Features

You can pass in features to cargo via `anchor test` by using the `features` input:

```yaml
steps:
  - uses: actions/checkout@v3
  - uses: metadaoproject/anchor-test@v2.3
    with: 
      anchor-version: '0.29.0'
      solana-cli-version: '1.18.26'
      node-version: '16.15.1'
      features: 'my-feature'
```

This defaults to 'default'.

## License

The scripts and documentation in this project are released under the [MIT License](LICENSE).
