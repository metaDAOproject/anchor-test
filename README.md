# Anchor Test

A fast and easy action for testing your Solana Anchor project.

# Usage

See [example-workflow.yml](example-workflow.yml)

You can optionally specify versions of Anchor, Node.js, and the Solana CLI tools. Below is an example with these parameters explicitly configured:

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
