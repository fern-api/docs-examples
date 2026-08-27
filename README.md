# docs-examples

Example Fern docs projects. Each top-level folder is a self-contained example with its own `fern/` configuration — browse the source on GitHub, or clone the repo to use one as a starting point for your own docs.

## Examples

<!-- Add new examples as a row in this table. Keep alphabetical. -->

| Example | Description | Live demo |
| --- | --- | --- |
| [`blog`](./blog) | Blog layout with authors, tags, images, and RSS/Atom/JSON feeds | [blog.docs.buildwithfern.com](https://blog.docs.buildwithfern.com) |
| [`docs-starter`](./docs-starter) | Minimal starter project | [docs-starter.docs.buildwithfern.com](https://docs-starter.docs.buildwithfern.com) |
| [`graphql`](./graphql) | GraphQL API Reference from a `.graphql` schema | [graphql.docs.buildwithfern.com](https://graphql.docs.buildwithfern.com) |
| [`grpc`](./grpc) | gRPC API Reference from `.proto` files | [grpc.docs.buildwithfern.com](https://grpc.docs.buildwithfern.com) |
| [`i18n`](./i18n) | Multi-language docs with English + Japanese translations | [i18n.docs.buildwithfern.com](https://i18n.docs.buildwithfern.com) |
| [`multi-source`](./multi-source) | Multi-source docs — six independent projects publishing to one domain with global theme, nested sub-paths, and shared branding | [multi-source.docs.buildwithfern.com](https://multi-source.docs.buildwithfern.com) |
| [`sse`](./sse) | SSE streaming API Reference with `x-fern-streaming` | [sse.docs.buildwithfern.com](https://sse.docs.buildwithfern.com) |
| [`versioning`](./docs-versioned) | Versioned site with a version dropdown and a shared page | [versioning.docs.buildwithfern.com](https://versioning.docs.buildwithfern.com) |

## Use an example

Clone the repo and copy the example folder you want:

```bash
git clone https://github.com/fern-api/docs-examples.git
cp -r docs-examples/<example> my-docs
cd my-docs
```

Then update `fern/fern.config.json` with your own organization name.
