# Medida Observada - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## Resource Profile: Medida Observada 

 
Registra as informações relacionadas a um tipo de observação. 

**Usos:**

* Refere a este Perfil: [Registro de Atendimento Clínico](StructureDefinition-BRRegistroAtendimentoClinico.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/br.gov.saude.rac.fhir|current/StructureDefinition/StructureDefinition-BRMedidaObservada.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-BRMedidaObservada.csv), [Excel](../StructureDefinition-BRMedidaObservada.xlsx), [Schematron](../StructureDefinition-BRMedidaObservada.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "BRMedidaObservada",
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
        "valueCanonical" : "https://fhir.saude.gov.br/fhir/r4/rac/1.0.0/ImplementationGuide/br.gov.saude.rac.fhir"
      }]
    }
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
    "valueCode" : "normative",
    "_valueCode" : {
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-conformance-derivedFrom",
        "valueCanonical" : "https://fhir.saude.gov.br/fhir/r4/rac/1.0.0/ImplementationGuide/br.gov.saude.rac.fhir"
      }]
    }
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
    "valueCode" : "4.0.1"
  }],
  "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada",
  "version" : "1.0.0-release",
  "name" : "BRMedidaObservada",
  "title" : "Medida Observada",
  "status" : "active",
  "date" : "2026-08-24T11:43:54-03:00",
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
  "description" : "Registra as informações relacionadas a um tipo de observação.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "workflow",
    "uri" : "http://hl7.org/fhir/workflow",
    "name" : "Workflow Pattern"
  },
  {
    "identity" : "sct-concept",
    "uri" : "http://snomed.info/conceptdomain",
    "name" : "SNOMED CT Concept Domain Binding"
  },
  {
    "identity" : "v2",
    "uri" : "http://hl7.org/v2",
    "name" : "HL7 v2 Mapping"
  },
  {
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  },
  {
    "identity" : "w5",
    "uri" : "http://hl7.org/fhir/fivews",
    "name" : "FiveWs Pattern Mapping"
  },
  {
    "identity" : "sct-attr",
    "uri" : "http://snomed.org/attributebinding",
    "name" : "SNOMED CT Attribute Binding"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Observation",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Observation",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Observation",
      "path" : "Observation"
    },
    {
      "id" : "Observation.extension",
      "path" : "Observation.extension",
      "slicing" : {
        "discriminator" : [{
          "type" : "value",
          "path" : "url"
        }],
        "rules" : "open"
      },
      "min" : 0
    },
    {
      "id" : "Observation.extension:measurementOrigin",
      "path" : "Observation.extension",
      "sliceName" : "measurementOrigin",
      "short" : "Origem da Medição Corpórea",
      "definition" : "Define a origem da medição corpórea adquirida.",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "Extension",
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BROrigemMedida"]
      }],
      "isModifier" : false
    },
    {
      "id" : "Observation.extension:usedClothes",
      "path" : "Observation.extension",
      "sliceName" : "usedClothes",
      "short" : "Roupas Usadas na Medição",
      "definition" : "Define o tipo de roupas usadas durante a medição corpórea.",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "Extension",
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRRoupasUsadasMedicao"]
      }],
      "isModifier" : false
    },
    {
      "id" : "Observation.identifier",
      "path" : "Observation.identifier",
      "max" : "0"
    },
    {
      "id" : "Observation.basedOn",
      "path" : "Observation.basedOn",
      "max" : "0"
    },
    {
      "id" : "Observation.partOf",
      "path" : "Observation.partOf",
      "max" : "0"
    },
    {
      "id" : "Observation.status",
      "path" : "Observation.status",
      "short" : "final | entered-in-error",
      "definition" : "O status da observação registrada.",
      "binding" : {
        "strength" : "required",
        "description" : "Código do Estado da Observação.",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BREstadoObservacao-1.0"
      }
    },
    {
      "id" : "Observation.category",
      "path" : "Observation.category",
      "max" : "0"
    },
    {
      "id" : "Observation.code",
      "path" : "Observation.code",
      "short" : "Tipo de Observação",
      "definition" : "Descreve o tipo de observação realizada.",
      "binding" : {
        "strength" : "required",
        "description" : "Código do Tipo de Observação.",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTipoObservacao-1.0"
      }
    },
    {
      "id" : "Observation.code.coding",
      "path" : "Observation.code.coding",
      "max" : "1"
    },
    {
      "id" : "Observation.subject",
      "path" : "Observation.subject",
      "type" : [{
        "code" : "Reference",
        "targetProfile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0"]
      }]
    },
    {
      "id" : "Observation.subject.extension",
      "path" : "Observation.subject.extension",
      "slicing" : {
        "discriminator" : [{
          "type" : "value",
          "path" : "url"
        }],
        "rules" : "open"
      },
      "min" : 0
    },
    {
      "id" : "Observation.subject.extension:unidentifiedPatient",
      "path" : "Observation.subject.extension",
      "sliceName" : "unidentifiedPatient",
      "short" : "Dados do Indivíduo Não Identificado",
      "min" : 0,
      "type" : [{
        "code" : "Extension",
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuoNaoIdentificado-1.0"]
      }],
      "mustSupport" : true
    },
    {
      "id" : "Observation.subject.extension:unidentifiedPatient.extension",
      "path" : "Observation.subject.extension.extension",
      "slicing" : {
        "discriminator" : [{
          "type" : "value",
          "path" : "url"
        }],
        "rules" : "open"
      },
      "min" : 3
    },
    {
      "id" : "Observation.subject.extension:unidentifiedPatient.extension:gender",
      "path" : "Observation.subject.extension.extension",
      "sliceName" : "gender",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Observation.subject.extension:unidentifiedPatient.extension:birthYear",
      "path" : "Observation.subject.extension.extension",
      "sliceName" : "birthYear",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Observation.subject.extension:unidentifiedPatient.extension:reason",
      "path" : "Observation.subject.extension.extension",
      "sliceName" : "reason",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Observation.subject.reference",
      "path" : "Observation.subject.reference",
      "max" : "0"
    },
    {
      "id" : "Observation.subject.type",
      "path" : "Observation.subject.type",
      "max" : "0"
    },
    {
      "id" : "Observation.subject.identifier.use",
      "path" : "Observation.subject.identifier.use",
      "max" : "0"
    },
    {
      "id" : "Observation.subject.identifier.value",
      "path" : "Observation.subject.identifier.value",
      "min" : 1
    },
    {
      "id" : "Observation.subject.identifier.period",
      "path" : "Observation.subject.identifier.period",
      "max" : "0"
    },
    {
      "id" : "Observation.subject.identifier.assigner",
      "path" : "Observation.subject.identifier.assigner",
      "max" : "0"
    },
    {
      "id" : "Observation.subject.display",
      "path" : "Observation.subject.display",
      "max" : "0"
    },
    {
      "id" : "Observation.focus",
      "path" : "Observation.focus",
      "max" : "0"
    },
    {
      "id" : "Observation.encounter",
      "path" : "Observation.encounter",
      "max" : "0"
    },
    {
      "id" : "Observation.effective[x]",
      "path" : "Observation.effective[x]",
      "type" : [{
        "code" : "Timing"
      }]
    },
    {
      "id" : "Observation.effective[x].code",
      "path" : "Observation.effective[x].code",
      "binding" : {
        "strength" : "required",
        "description" : "Frequência do uso de substância nos últimos 3 meses",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRFrequenciaUsoSubstancia"
      }
    },
    {
      "id" : "Observation.issued",
      "path" : "Observation.issued",
      "max" : "0"
    },
    {
      "id" : "Observation.performer",
      "path" : "Observation.performer",
      "max" : "0"
    },
    {
      "id" : "Observation.value[x]",
      "path" : "Observation.value[x]",
      "type" : [{
        "code" : "Quantity"
      },
      {
        "code" : "CodeableConcept"
      },
      {
        "code" : "dateTime"
      }]
    },
    {
      "id" : "Observation.dataAbsentReason",
      "path" : "Observation.dataAbsentReason",
      "max" : "0"
    },
    {
      "id" : "Observation.interpretation",
      "path" : "Observation.interpretation",
      "max" : "0"
    },
    {
      "id" : "Observation.note",
      "path" : "Observation.note",
      "max" : "1"
    },
    {
      "id" : "Observation.bodySite",
      "path" : "Observation.bodySite",
      "binding" : {
        "strength" : "required",
        "description" : "Local de Aferição",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRLocalAfericao-1.0"
      }
    },
    {
      "id" : "Observation.method",
      "path" : "Observation.method",
      "binding" : {
        "strength" : "required",
        "description" : "Posição em relação à gravidade.",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRPosicaoIndividuo"
      }
    },
    {
      "id" : "Observation.method.coding",
      "path" : "Observation.method.coding",
      "max" : "1"
    },
    {
      "id" : "Observation.specimen",
      "path" : "Observation.specimen",
      "max" : "0"
    },
    {
      "id" : "Observation.device",
      "path" : "Observation.device",
      "max" : "0"
    },
    {
      "id" : "Observation.referenceRange",
      "path" : "Observation.referenceRange",
      "max" : "0"
    },
    {
      "id" : "Observation.hasMember",
      "path" : "Observation.hasMember",
      "max" : "0"
    },
    {
      "id" : "Observation.derivedFrom",
      "path" : "Observation.derivedFrom",
      "max" : "0"
    },
    {
      "id" : "Observation.component",
      "path" : "Observation.component",
      "max" : "1"
    }]
  }
}

```
