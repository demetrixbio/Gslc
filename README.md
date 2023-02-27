#Genotype Specification Language (GSL)

## Building GSL

* get the dotnet sdk 7.0 installed
* `./build.sh`  (recommend bash shell on windows) 
* compiler ends up in `bin/Gslc/net7.0/Gslc.exe`

## Running GSL

```
$ bin/Gslc/net7.0/Gslc.exe --snapgene . foo examples/simple_fusion.gsl
```

```
$ bin/Gslc/net7.0/Gslc.exe --snapgene . foo examples/simple_fusion.gsl
// GSL core compiler version 0.5.0 (04b205)
Writing snapgene output to dir=. tag=foo path=.\foo.0.dna
```

Open up `foo.0.dna` with your favorite genbank viewer  (e.g. [snapgene](https://www.snapgene.com/snapgene-viewer) )


## Intro
This is the command line wrapper around the main GslCore library that implements the bulk of the compiler.

## NOTE

This version builds against the public Dmx.GslCore library (vs the Amyris GslCore)

## Overview

Amyris domain specification language for rapidly specifying genetic designs

Documentation in the repo is sparse currently, but you can find

* the scientific paper describing the language here http://pubs.acs.org/doi/abs/10.1021/acssynbio.5b00194
* GSL documentation as part of the Autodesk genetic constructor tool here https://geneticconstructor.readme.io/docs/genotype-specification-language
* the press release on the GSL / Autodesk collaboration here http://investors.amyris.com/releasedetail.cfm?ReleaseID=992005
