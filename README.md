# wdio-ts-native-repro

Reproduces a TS1540 error when using `@wdio/globals` with `@typescript/native-preview` (tsgo).

## Setup

Install [pnpm](https://pnpm.io/) if you don't have it:

```sh
npm install -g pnpm
```

Then install dependencies:

```sh
pnpm install
```

## Reproduce

```sh
pnpm typecheck
```

This runs `tsgo --noEmit` and should surface the TS1540 error from `@wdio/globals/types`.