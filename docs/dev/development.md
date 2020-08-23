# Development

## Steps

### Component testing
```sh
make <component> action=test
```

### Publishing to local PyPi repository
```sh
make <component> action=publish
```

### Release component version
```sh
make <component> action=release
```

### Patch component version
```sh
make <component> action=patch
```

## Usage

### How to release component

Before releasing the component check that there are no uncommited code 
```sh
git status
```
and the all tests are passed
```sh
make <component> action=test
```
Change the compoment version to the release version
```sh
make <component> action=release
```
If the previos step is successful, commit version changes and create new tag
```sh
git commit -m '[+] <component>-<version>'
git tag -a '<component>-<version>' -m '<component>-<version>'
```
Make new patch version
```sh
make <component> action=patch
```
and commit version changes
```sh
git commit -m '[+] <component>-<version>'
```
where version with `dev0` suffix
