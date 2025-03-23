# Bun Runtime for AWS Lambda

This repository provides [Bun](https://bun.sh/) as an AWS Lambda runtime layer. It enables running JavaScript and TypeScript applications on AWS Lambda using Bun.

> [!NOTE]
> This is Bun itself packaged as a Lambda layer, not the special Lambda runtime layer that Bun provides. If you need that layer, you can find instructions over at [oven-sh/bun/packages/bun-lambda](https://github.com/oven-sh/bun/tree/main/packages/bun-lambda)

## Available Layers

Two architecture layers are available:

#### BunRuntimeArm64
`arn:aws:lambda:us-east-1:582637575117:layer:BunRuntimeArm64:1`

#### BunRuntimeX64 
`arn:aws:lambda:us-east-1:582637575117:layer:BunRuntimeX64:1`

## Automatic Updates

[Check Bun Version](https://github.com/sumcoding/bun-runtime/actions/workflows/check-bun-version.yml)

This repository automatically checks for new Bun releases on the first day of each month. When a new version is detected:

1. GitHub Actions builds the new layer packages
2. Deploys them to AWS as a new version

## License

MIT

## Author 
@sumcoding
