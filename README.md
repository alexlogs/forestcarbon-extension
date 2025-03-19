# Forest Carbon Extension Specification

- **Title:** Forest Carbon
- **Identifier:** <https://fiboa.github.io/forestcarbon-template/v0.1.0/schema.yaml>
- **Property Name Prefix:** forestcarbon
- **Extension Maturity Classification:** Proposal
- **Owner**: @alexlogs

This document explains the forestcarbon Extension to the
[Field Boundaries for Agriculture (fiboa) Specification](https://github.com/fiboa/specification).

The ForestCarbon Extension is a specification to support forest carbon projects. This extension provides a standardized schema for representing forest carbon projects and their boundaries in alignment with carbon registries and methodologies.

This builds off a database that was built for a global database of nature-based carbon offset project boundaries. You can read the [preprint here](https://www.researchsquare.com/article/rs-4535931/v1) and find the [dataset here](https://zenodo.org/records/11459391).

- Examples:
  - [GeoJSON](examples/geojson/)
  - [GeoParquet](examples/geoparquet/)
- [Schema](schema/schema.yaml)
- [Changelog](./CHANGELOG.md)

## Properties

The properties in the table below can be used in these parts of fiboa documents:

- [ ] Collection
- [x] Feature Properties

| Property Name | Type | Description |
| ------------- | ---- | ----------- |
| forestcarbon:projectName | string | The name of the carbon project as given in the documentation. |
| forestcarbon:projectID | string | A combination of the registry abbreviation and project number. |
| forestcarbon:registryName | string | The name of the registry where project information is hosted. Possible values are: American Carbon Registry, BioCarbon Registry, Climate Action Reserve, EcoRegistry, Gold Standard, Verra. |
| forestcarbon:methodology | string | **REQUIRED**. The name of the methodology used for the project's implementation. |
| forestcarbon:projectType | string | **REQUIRED**. The type of forestry carbon offset program. One of the following: ARR, AD, IFM. |
| forestcarbon:country | string | The country where the project is located. |
| forestcarbon:projectDeveloperName | string | Name of the entity or individual organizing, proposing, or advocating a particular carbon offset project. |
| forestcarbon:projectStartDate | string | Date of the start of the crediting period (ISO 8601 format). |
| forestcarbon:projectEndDate | string | Date of the end of the crediting period (ISO 8601 format). |
| forestcarbon:dateOfEntry | string | Date when the project information was added to the database (ISO 8601 format). |
| forestcarbon:processingApproach | string | Method used to obtain boundary data. One of: Official, Georeferenced, Linear, Method. |
| forestcarbon:pdDeclinedToProvide | string | Whether the project developer declined to provide geometry information. One of: Yes, No, N/A. |
| forestcarbon:geometryType | string | Indicates if the geometry is a point or a polygon. |

## Contributing

See the [contributing guideline](CONTRIBUTING.md) for more details.
