# gx-js

a distributed package manager for javascript, built on [gx](https://github.com/whyrusleeping/gx)

## installation

you will need [go-ipfs](https://github.com/ipfs/go-ipfs) > 0.4.0 and [gx](https://github.com/whyrusleeping/gx) > 0.4.0

then, you can just

      gx install --global [gx-js-hash-to-come]

## usage

      gx-js install [package]
    
will install packages to `./node-modules/` recursively, from ipfs if possible, otherwise from npm.

if no package is specified, will install each package in `package.json`
    
    gx-js publish [-r depth]
    
publishes to the gx npm repository. the -r flag will recursively publish dependencies to ipfs, up to some maximum depth (0 to publish full dependency tree).
    
if -r is ommitted, it will publish your package to ipfs, but keep your dependencies on npm.
    
    gx-js init 

see npm init

## license

BSD
