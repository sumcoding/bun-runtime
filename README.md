# Bun Runtime for AWS Lambda

This repository provides [Bun](https://bun.sh/) as an AWS Lambda runtime layer. It enables running JavaScript and TypeScript applications on AWS Lambda using Bun.

> [!TIP]
> This is Bun itself packaged as a Lambda layer, not the special Lambda runtime layer that Bun provides. If you need that layer, you can find instructions over at [oven-sh/bun/packages/bun-lambda](https://github.com/oven-sh/bun/tree/main/packages/bun-lambda)

## Available Layers

Two architecture layers are available:
| Layer Name      | Arch  | ARN                                                             |
|-----------------|-------|-----------------------------------------------------------------|
| BunRuntimeArm64 | ARM64 | `arn:aws:lambda:{region}:582637575117:layer:BunRuntimeArm64:{version}` |
| BunRuntimeX64   | X64   | `arn:aws:lambda:{region}:582637575117:layer:BunRuntimeX64:{version}`   |

## Automatic Updates

[Check Bun Version](https://github.com/sumcoding/bun-runtime/actions/workflows/check-bun-version.yml)

This repository automatically checks for new Bun releases on the first day of each month. When a new version is detected:

1. GitHub Actions builds the new layer packages
2. Deploys them to AWS regions as a new version

> [!NOTE]
> The version of Bun in the layer may be behind the version in the bun repo and there will not be a corresponding layer version for every version of bun released.

## Author 
@sumcoding
