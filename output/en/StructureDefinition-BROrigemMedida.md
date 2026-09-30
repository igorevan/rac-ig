# Origem da Medição - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## Extension: Origem da Medição 

Extensão para incluir a origem da medição corpórea (altura e peso).

**Context of Use**

**Usage info**

**Usos:**

* Usa este Extensão: [Medida Observada](StructureDefinition-BRMedidaObservada.md)
* Exemplos para este Extensão: [Bundle/bundle-example-rac-1](Bundle-bundle-example-rac-1.md), [Bundle/bundle-example-rac-2](Bundle-bundle-example-rac-2.md) and [Bundle/bundle-example-rac-tc](Bundle-bundle-example-rac-tc.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/br.gov.saude.rac.fhir|current/StructureDefinition/StructureDefinition-BROrigemMedida.json)

### Formal Views of Extension Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-BROrigemMedida.csv), [Excel](../StructureDefinition-BROrigemMedida.xlsx), [Schematron](../StructureDefinition-BROrigemMedida.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "BROrigemMedida",
  "language" : "pt-BR",
  "extension" : [{
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-wg",
    "valueCode" : "ehr"
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-fmm",
    "valueInteger" : 1,
    "_valueInteger" : {
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-conformance-derivedFrom",
        "valueCanonical" : "https://fhir.saude.gov.br/rac/ImplementationGuide/br.gov.saude.rac.fhir"
      }]
    }
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
    "valueCode" : "normative",
    "_valueCode" : {
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-conformance-derivedFrom",
        "valueCanonical" : "https://fhir.saude.gov.br/rac/ImplementationGuide/br.gov.saude.rac.fhir"
      }]
    }
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
    "valueCode" : "4.0.1"
  }],
  "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BROrigemMedida",
  "version" : "1.0.0-release",
  "name" : "BROrigemMedida",
  "title" : "Origem da Medição",
  "status" : "active",
  "experimental" : false,
  "date" : "2026-09-30T18:22:16-03:00",
  "publisher" : "Ministério da Saúde do Brasil",
  "contact" : [{
    "name" : "Ministério da Saúde do Brasil",
    "telecom" : [{
      "system" : "url",
      "value" : "http://www.saude.gov.br"
    },
    {
      "system" : "email",
      "value" : "cgiis.datasus@saude.gov.br"
    }]
  }],
  "description" : "Extensão para incluir a origem da medição corpórea (altura e peso).",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  }],
  "kind" : "complex-type",
  "abstract" : false,
  "context" : [{
    "type" : "element",
    "expression" : "Observation"
  }],
  "type" : "Extension",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Extension",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Extension.url",
      "path" : "Extension.url",
      "fixedUri" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BROrigemMedida"
    },
    {
      "id" : "Extension.value[x]",
      "path" : "Extension.value[x]",
      "short" : "Código da Medição Corpórea",
      "type" : [{
        "code" : "CodeableConcept"
      }],
      "binding" : {
        "strength" : "required",
        "description" : "Origem da Medição Corpórea",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BROrigemMedida"
      }
    },
    {
      "id" : "Extension.value[x].coding",
      "path" : "Extension.value[x].coding",
      "max" : "1"
    }]
  }
}

```
