# bun-add-bug

To reproduce the bug where the postinstall script does not behave like `bun install`, run `bun add` in the workspace `package-a`:

```bash
bun install # it works fine

cd packages/package-a
bun add -d react # postinstall scripts cannot be found
```

