# PackageRegistry
A package registry for Julia packages developed under this GitHub org.

## Add Registry

To activate the registry, do
```
using Pkg
pkg"registry add git@github.com:New-Earth-Lab/PackageRegistry.git"
```
This only needs to be done once per Julia installation.

## Register a Package or a New Version of a Package

The recommended way to register a package or a new version of a
package is simply:

```
using LocalRegistry
register()
```

For this to work you need to either have the package in your current
directory or have the package activated.

Actually there are some more requirements but those are usually
satisfied. Read more about that, a number of options to customize the
call, and some additional features in the [detailed
instructions](https://github.com/GunnarFarneback/LocalRegistry.jl/blob/master/docs/register.md).
