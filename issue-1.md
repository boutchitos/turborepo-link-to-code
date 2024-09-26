This command:
```bash
pnpm dlx create-turbo@canary --example basic
```
generates

```bash
ls my-turbo-basic/packages
eslint-config     typescript-config ui
```

But this command:
```bash
pnpm dlx create-turbo@canary --example with-vite
```
generates

```bash
ls my-turbo-with-vite/packages
config-eslint     config-typescript ui
```

There is an inconsistency regarding config folders naming. I did not try the other examples.

This also breaks the documentation from this guide: [Use a base tsconfig file](https://turbo.build/repo/docs/guides/tools/typescript#use-a-base-tsconfig-file)

>Inside `packages/tsconfig`, we have a few json ...

`tsconfig` is not such a folder.
