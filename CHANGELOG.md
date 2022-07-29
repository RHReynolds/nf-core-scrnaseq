# nf-core/scrnaseq: Changelog

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Unreleased on nf-core/scrnaseq#dev

* [#92f7555](https://github.com/RHReynolds/nf-core-scrnaseq/commit/92f7555f73a703e56631fa9a8a80bceb0da961a7) Merge FASTQ files from the same sample.
* [#67](https://github.com/nf-core/scrnaseq/pull/67) Fix bug causing processing of only one sample
* [#b5fb831](https://github.com/RHReynolds/nf-core-scrnaseq/commit/b5fb83162f18193a3422c7af6fe61ed790134b63) Add STARsolo files as optional outputs

## v2.0.1dev

### Fixes

- Fixed Kallistobustools workflow [#123](https://github.com/nf-core/scrnaseq/issues/123) by upgrading to nf-core/modules module

## v2.0.0 - 2022-06-17 "Gray Nickel Beagle"

- Pipeline ported to dsl2
- Template update with latest nf-core/tools v2.1
- Added cellranger v.7.0.0 subworkflow
- Added full size tests

### Fixes

- Make sure pipeline runs on multiple samples [#77](https://github.com/nf-core/scrnaseq/pull/77)
- Fix issue where STARsolo always uses 10XV2 chemistry [#60](https://github.com/nf-core/scrnaseq/issues/60)

## v1.1.0 - 2021-03-24 "Olive Mercury Corgi"

- Template update with latest nf-core/tools v1.13.2
- Parameters JSON Schema added [#42](https://github.com/nf-core/scrnaseq/issues/42)
- [25](https://github.com/nf-core/scrnaseq/issues/25) Fix small documentation error with wrong parameter for txp2gene

### Fixes

- [#20](https://github.com/nf-core/scrnaseq/issues/20) Fix Transcriptome Fasta argument not detected well
- [#21](https://github.com/nf-core/scrnaseq/issues/21) Fix `--kallisto_index` being ignored

## v1.0.0 - 2019-11-28 "Tiny Aluminium Crab"

Initial release of nf-core/scrnaseq, created with the [nf-core](http://nf-co.re/) template.
This includes the following workflow options:

- Salmon Alevin + AlevinQC
- STARSolo
- Kallisto / BUStools
