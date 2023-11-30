# Getting Started With Schematics

This repository is a basic Schematic implementation that serves as a starting point to create and publish Schematics to NPM.

### Testing

To test locally, install `@angular-devkit/schematics-cli` globally and use the `schematics` command line tool. That tool acts the same as the `generate` command of the Angular CLI, but also has a debug mode.

Check the documentation with

```bash
schematics --help
```

## Create new 

```
schematics blank --name=<schematics-name>
```

### Unit Testing

`npm run test` will run the unit tests, using Jasmine as a runner and test framework.

### Publishing

To publish, simply do:

```bash
npm run build
npm publish
```

Debugging
In order to debug your schematics, you need to run with node in debugging mode:
```bash
node --inspect-brk $(which schematics) .:myComponent --name=test
```


## References

1. [Create Angular Schematics](https://blog.angular.io/schematics-an-introduction-dc1dfbc2a2b2)

That's it!
