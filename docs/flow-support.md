# Flow Support

To use flowtype with the public api of styled-components we recommend that
you use the library definition in [flow-typed].

To install it you can use the flow-typed cli or download it manually from
the git repository and storing it in a flow-typed folder in the same folder
as your flowconfig.

### Ignore node_modules/styled-components

To make sure flow will completely ignore any files from the original styled-components package, add this to your `.flowconfig`:

```ini
[ignore]
.*/node_modules/styled-components/.*
```

### Installing the libdef with flow-typed

```shell
npm i -g flow-typed # if you do not already have flow-typed
flow-typed install styled-components@<version>
```

[flow-typed]: https://github.com/flowtype/flow-typed


### Troubleshooting

By default, if your `.flowconfig` contains an empty `[libs]` section, it will assume `<PROJECT_ROOT>/flow-typed/.*` as your default libdef path.

If you already configured some other `[libs]` paths, make sure to add `flow-typed/` as well:

```ini
[libs]
some/other/libs/.*
flow-typed
```
