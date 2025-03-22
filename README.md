# Forestcarbon Extension Specficiation

- **Title:** forestcarbon
- **Identifier:** <https://vecorel.github.io/forestcarbon-template/v0.1.0/schema.yaml>
- **Property Name Prefix:** forestcarbon
- **Extension Maturity Classification:** Proposal
- **Owner**: @alexlogs

This document explains the forestcarbon to the
[Vecorel Specification](https://github.com/vecorel/specification).

The ForestCarbon Extension is a specification to support forest carbon projects. This extension provides a standardized schema for representing forest carbon projects and their boundaries in alignment with carbon registries and methodologies.

- Examples:
  - [GeoJSON](examples/geojson/)
  - [GeoParquet](examples/geoparquet/)
- [Schema](schema/schema.yaml)
- [Changelog](./CHANGELOG.md)

## Properties

The properties in the table below can be used in these parts of Vecorel documents:

- [ ] Collection
- [x] Feature Properties

| Property Name   | Type   | Description |
| --------------- | ------ | ----------- |
| forestcarbon:projectName | string | The name of the carbon project as given in the documentation |
| forestcarbon:projectID | string  | A combination of the registry abbreviation and project number |
| forestcarbon:registryName | string  | The name of the registry where project information is hosted |
| forestcarbon:methodology | string  | The name of the methodology used for the project’s implementation |
| forestcarbon:projectType | string  | The type of forestry carbon offset program |
| forestcarbon:country | string  | The country where the project is located |
| forestcarbon:projectDeveloperName | string  | Name of the entity or individual organizing, proposing, or advocating a particular carbon offset project. In case of multiple entities/individuals, only the first name is recorded here |
| forestcarbon:projectStartDate | date  | Date of the start of the crediting period |
| forestcarbon:projectEndDate | date  | Date of the end of the crediting period |
| forestcarbon:processingApproach | string  | One of four possible values: Official, Georeferenced, Linear, or Method. |




## Contributing

See the [contributing guideline](CONTRIBUTING.md) for more details.
