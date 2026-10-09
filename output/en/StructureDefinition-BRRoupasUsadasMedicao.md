# Roupas Usadas na Medição - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## Extension: Roupas Usadas na Medição 

**Context of Use**

**Usage info**

**Usos:**

* Usa este Extensão: [Medida Observada](StructureDefinition-BRMedidaObservada.md)
* Exemplos para este Extensão: [Bundle/bundle-example-rac-1](Bundle-bundle-example-rac-1.md), [Bundle/bundle-example-rac-2](Bundle-bundle-example-rac-2.md) and [Bundle/bundle-example-rac-tc](Bundle-bundle-example-rac-tc.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/br.gov.saude.rac.fhir|current/StructureDefinition/StructureDefinition-BRRoupasUsadasMedicao.json)

### Formal Views of Extension Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-BRRoupasUsadasMedicao.csv), [Excel](../StructureDefinition-BRRoupasUsadasMedicao.xlsx), [Schematron](../StructureDefinition-BRRoupasUsadasMedicao.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "BRRoupasUsadasMedicao",
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
  "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRRoupasUsadasMedicao",
  "version" : "1.0.0-release",
  "name" : "BRRoupasUsadasMedicao",
  "title" : "Roupas Usadas na Medição",
  "status" : "active",
  "experimental" : false,
  "date" : "2026-10-08T20:36:58-03:00",
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
  "description" : "Descreve o tipo de roupas usadas durante a medição com base no código LOINC 8352-7.",
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
      "fixedUri" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRRoupasUsadasMedicao"
    },
    {
      "id" : "Extension.value[x]",
      "path" : "Extension.value[x]",
      "short" : "Código do tipo de roupa usada para medição corpórea",
      "type" : [{
        "code" : "CodeableConcept"
      }],
      "binding" : {
        "strength" : "required",
        "description" : "Roupas Usadas na Medição Corpórea",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/RoupasUsadasMedicao"
      }
    }]
  }
}

```
