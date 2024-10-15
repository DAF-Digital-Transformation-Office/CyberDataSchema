# Cyber Data Schema (CDS)

Welcome to the Cyber Digital Revolution! The Cyber Data Schema (CDS) is the foundation for the project and was initially developed to facilitate the digital transformation of cybersecurity assessment and authorization content through a relationally-joined database. The CDS is a comprehensive collection of data elements and attributes designed to represent relevant content in a machine-readable and queriable format.

## Features

- **Extensibility**: The CDS is designed to be easily extended to support new types of assessment and authorization content.
- **Interoperability**: The CDS can be used to exchange cyber content between different organizations, systems and tools.
- **Data Standardization/Normalization**: The CDS uses minimally viable elements to standardize and normalize cybersecurity assessment and authorization content.
- **Assessment Automation**: The CDS aims to enable for automation of assessment toolchains by providing a common data model for cybersecurity content.

## Contributing

We welcome contributions to the Cyber Data Schema! If you'd like to contribute, please get involved however suites you best: reporting bugs, requesting features, or submitting pull requests.

## License

The Cyber Data Schema is licensed under the Apache 2.0 Commons License. See the `LICENSE` file for more information.

## Acknowledgements

We'd like to thank all the contributors who have helped make the Cyber Data Schema possible. 


## Version Control

### Major Version Update
Increase the major version when you make incompatible API changes or schema changes. This includes removing or renaming fields, changing the data type of existing fields, or making other changes that would break backward compatibility.
- **Delete Table**: Removes an entire table, breaking any implementations that depend on its existence.
- **Delete Column**: Removes a column, affecting data structure and any dependencies on that column.
- **Delete Relationship**: Removes a relationship, potentially breaking dependencies between tables.
- **Edit Column Type**: Changes the fundamental data type or expected data structure of a column.
- **Delete Column Type**: Removing a defined column type affects columns dependent on this type.
- **Delete Relationship Type**: Removing a relationship type impacts all relationships utilizing this type.

### Minor Version Update
Increase the minor version when you add functionality in a backward-compatible manner. This can include adding new fields or new tables, or perhaps introducing new optional features in the schema that do not disturb existing data and functionality.
- **Add Table**: Introduces a new table without affecting existing ones.
- **Add Column**: Adds a new column without altering existing columns' behavior.
- **Add Relationship**: Introduces new relationships without changing existing ones.
- **Add Column Type**: Adds a new type for columns, which doesn’t affect existing columns.
- **Add Relationship Type**: Adds a new type for defining relationships, enhancing schema capabilities.
- **Edit Table (name, description, coordinates)**: Changes that do not affect the table’s structure.
- **Edit Column (name, description, properties)**: Changes that don’t affect the fundamental behavior of the column.
- **Edit Relationship (type, table_uuid, column_uuid, description)**: Modifies details of a relationship but doesn't remove it or change its fundamental linking behavior.

### Patch Version Update
Increase the patch version when you make backward-compatible bug fixes. This is typically reserved for small changes that fix errors in the existing schema without adding new features or changing the behavior of the system.
- **Add/Edit table description, type, or coordinates**: Minor updates for better clarity or correction of typos.
- **Edit name or description**: Updates for clarity or correction of errors in metadata.
- **Edit relationship description**: Minor textual corrections or updates for clarity.
