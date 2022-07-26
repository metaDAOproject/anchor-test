# Anchor Test

A fast and easy action for testing your Solana Anchor project.

# Usage

See [action.yml](action.yml). You can specify versions of anchor, node.js, and the solana cli tools. If you don't specify a version for any of these, the action will use a pre-defined default. An example with these parameters explicitly configued is below:

```yaml
steps:
  - uses: actions/checkout@v3
  - uses: metadaobuilders/anchor-test@v1
    with: 
      anchor-version: '0.24.2' 
      solana-cli-version: '1.10.32'
      node-version: '16.15.1'
```

# License

The scripts and documentation in this project are released under the [GNU General Public License](LICENSE).
