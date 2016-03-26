# gx-js

a distributed package manager for javascript, built on [gx](https://github.com/whyrusleeping/gx)

## usage

        gx-js install [package]
    
    will install packages to `./node-modules/` recursively, from ipfs if possible, otherwise from npm.
    
    if no package is specified, will install each package in `package.json`
    
        gx-js publish [name] [-r depth]
    
    publishes to the gx npm repository. the -r flag will recursively publish dependencies to ipfs, up to some maximum depth (0 to publish full dependency tree).
    
    if -r is ommitted, it will publish your package to ipfs, but keep your dependencies on npm.
    
        gx-js init 

    see npm init

## license

BSD
