# BSI CycloneDX Property Taxonomy, v0.1.0

This is the official [BSI](https://www.bsi.bund.de/EN/Home/home_node.html) (German Federal Office for Information Security) property taxonomy for CycloneDX.

For more information about CycloneDX property taxonomies, see [CycloneDX documentation](https://github.com/CycloneDX/cyclonedx-property-taxonomy).

The key words “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”, “SHOULD NOT”, “RECOMMENDED”, “NOT RECOMMENDED”, “MAY”, and “OPTIONAL” in this document are to be interpreted as described in [BCP 14](https://www.rfc-editor.org/info/bcp14) ([RFC 2119](https://www.rfc-editor.org/rfc/rfc2119), [RFC 8174](https://www.rfc-editor.org/rfc/rfc8174)) when, and only when, they appear in all capitals, as shown here.

## `bsi` Namespace Taxonomy

| Namespace | Description |
| --- | --- |
| **`bsi:component`** | Namespace for properties associated with components |

## `bsi:component` Namespace Taxonomy

| Property | Description |
| --- | --- |
| **`bsi:component:executable`** | A flag indicating whether the component is executable; possible values are `executable` and `non-executable`; see also section 5.2.2 of BSI TR-03183-2 v2.0.0. For additional explanation see section 8.1.3 of BSI TR-03183-2 v2.0.0.<br />Only valid for use in `components[]/properties` and `metadata/component/properties`. MUST occur exactly once per component. |
| **`bsi:component:archive`** | A flag indicating whether the component is an archive; possible values are `archive` and `no archive`; see also section 5.2.2 of BSI TR-03183-2 v2.0.0. For additional explanation see section 8.1.4 of BSI TR-03183-2 v2.0.0.<br />Only valid for use in `components[]/properties` and `metadata/component/properties`. MUST occur exactly once per component. |
| **`bsi:component:structured`** | A flag indicating whether the component is a structured file; i.e. metadata of the contents is still present (see section 3.2.1); possible values are `structured` and `unstructured`; see also section 5.2.2 of BSI TR-03183-2 v2.0.0. If a component contains both structured and unstructured parts the value `structured` MUST be used. For additional explanation see section 8.1.5 of BSI TR-03183-2 v2.0.0.<br />Only valid for use in `components[]/properties` and `metadata/component/properties`. MUST occur exactly once per component. |
| **`bsi:component:filename`** | A field providing the actual filename of the component (i.e. not its path); see also section 5.2.2 of BSI-TR-03183-2 v2.0.0. For additional explanation see section 3.2.1 of BSI TR-03183-2 v2.0.0.<br />Only valid for use in `components[]/properties` and `metadata/component/properties`. MUST occur at most once per component. |
| **`bsi:component:associatedLicences`** | A field providing the associated licence(s) of the component as a single licence identifier or licence expression from the perspective of the SBOM creator; see also section 5.2.2 of BSI TR-03183-2 v2.0.0. For additional explanation see sections 6.1 and 8.1.9 of BSI TR-03183-2 v2.0.0.<br />Only valid for use in `components[]/properties` and `metadata/component/properties`. MUST occur exactly once per component. |

## Contributing

These properties are maintained by BSI. Feel free to open an issue in this source code repository, if you have any questions, contributions or suggestions.

## Licence

© Copyright 2024 German Federal Office for Information Security (BSI)

Licensed under [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0).
