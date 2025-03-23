# Bun Runtime for AWS Lambda

This repository provides [Bun](https://bun.sh/) as an AWS Lambda runtime layer.

> Note:
> This is Bun itself packaged as a Lambda layer, not the special Lambda runtime layer that Bun provides. If you need that layer, you can find instructions over at [oven-sh/bun/packages/bun-lambda](https://github.com/oven-sh/bun/tree/main/packages/bun-lambda)

## Available Layers

Two architecture layers are included:

#### BunRuntimeArm64
`arn:aws:lambda:{region}:{account}:layer:BunRuntimeArm64:1`

#### BunRuntimeX64 
`arn:aws:lambda:{region}:{account}:layer:BunRuntimeX64:1`

## License

MIT

## Author 
@sumcoding
