# Flow Support

To use flowtype with the public api of styled-components we recommend that
you use the library definition in [flow-typed].

To install it you can use the flow-typed cli or download it manually from
the git repository and storing it in a flow-typed folder in the same folder
as your flowconfig.

### Installing the libdef with flow-typed

```shell
npm i -g flow-typed # if you do not already have flow-typed
flow-typed install styled-components@<version>
```

[flow-typed]: https://github.com/flowtype/flow-typed
