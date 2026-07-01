# Medicamento - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## Resource Profile: Medicamento 

 
Medicamento 

**Usos:**

* Refere a este Perfil: [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) and [Registro de Prescrição de Medicamento](StructureDefinition-BRRegistroPrescricaoMedicamento.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/br.gov.saude.rac.fhir|current/StructureDefinition/StructureDefinition-BRMedicamento.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-BRMedicamento.csv), [Excel](../StructureDefinition-BRMedicamento.xlsx), [Schematron](../StructureDefinition-BRMedicamento.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "BRMedicamento",
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
  "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedicamento",
  "version" : "1.0.0-release",
  "name" : "BRMedicamento",
  "title" : "Medicamento",
  "status" : "active",
  "experimental" : false,
  "date" : "2026-06-26T11:16:11-03:00",
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
  "description" : "Medicamento",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "script10.6",
    "uri" : "http://ncpdp.org/SCRIPT10_6",
    "name" : "Mapping to NCPDP SCRIPT 10.6"
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
    "identity" : "v2",
    "uri" : "http://hl7.org/v2",
    "name" : "HL7 v2 Mapping"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Medication",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Medication",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Medication",
      "path" : "Medication"
    },
    {
      "id" : "Medication.id",
      "path" : "Medication.id",
      "max" : "0"
    },
    {
      "id" : "Medication.implicitRules",
      "path" : "Medication.implicitRules",
      "max" : "0"
    },
    {
      "id" : "Medication.language",
      "path" : "Medication.language",
      "max" : "0"
    },
    {
      "id" : "Medication.text",
      "path" : "Medication.text",
      "max" : "0"
    },
    {
      "id" : "Medication.contained",
      "path" : "Medication.contained",
      "max" : "0"
    },
    {
      "id" : "Medication.extension",
      "path" : "Medication.extension",
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
      "id" : "Medication.extension:serialCode",
      "path" : "Medication.extension",
      "sliceName" : "serialCode",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "Extension",
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRCodigoSerialMedicamento"]
      }]
    },
    {
      "id" : "Medication.identifier",
      "path" : "Medication.identifier",
      "max" : "0"
    },
    {
      "id" : "Medication.code",
      "path" : "Medication.code",
      "short" : "Nome do Medicamento",
      "definition" : "Nome e terminologia do medicamento fabricado.",
      "min" : 1,
      "binding" : {
        "strength" : "preferred",
        "description" : "Define a terminologia de um dado medicamento.",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTerminologiaMedicamento"
      }
    },
    {
      "id" : "Medication.code.id",
      "path" : "Medication.code.id",
      "max" : "0"
    },
    {
      "id" : "Medication.code.coding",
      "path" : "Medication.code.coding",
      "min" : 1,
      "max" : "1"
    },
    {
      "id" : "Medication.code.coding.id",
      "path" : "Medication.code.coding.id",
      "max" : "0"
    },
    {
      "id" : "Medication.code.coding.system",
      "path" : "Medication.code.coding.system",
      "min" : 1
    },
    {
      "id" : "Medication.code.coding.version",
      "path" : "Medication.code.coding.version",
      "short" : "Versão da terminologia - se relevante"
    },
    {
      "id" : "Medication.code.coding.code",
      "path" : "Medication.code.coding.code",
      "min" : 1
    },
    {
      "id" : "Medication.code.coding.display",
      "path" : "Medication.code.coding.display",
      "max" : "0"
    },
    {
      "id" : "Medication.code.coding.userSelected",
      "path" : "Medication.code.coding.userSelected",
      "max" : "0"
    },
    {
      "id" : "Medication.code.text",
      "path" : "Medication.code.text",
      "short" : "Nome da terminologia"
    },
    {
      "id" : "Medication.status",
      "path" : "Medication.status",
      "binding" : {
        "strength" : "required",
        "description" : "Estado da Solicitação de Medicamento",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BREstadoSolicitacaoMedicamento-1.0"
      }
    },
    {
      "id" : "Medication.manufacturer",
      "path" : "Medication.manufacturer",
      "max" : "0"
    },
    {
      "id" : "Medication.form",
      "path" : "Medication.form",
      "short" : "Unidade de medida do medicamento",
      "definition" : "Unidade de medida do medicamento prescrito (ex.: comprimido, cápsula, frasco, caixa etc.).",
      "min" : 1,
      "binding" : {
        "strength" : "required",
        "description" : "Unidade de medida do medicamento",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRUnidadeMedidaMedicamento"
      }
    },
    {
      "id" : "Medication.amount",
      "path" : "Medication.amount",
      "max" : "0"
    },
    {
      "id" : "Medication.ingredient",
      "path" : "Medication.ingredient",
      "max" : "0"
    },
    {
      "id" : "Medication.batch",
      "path" : "Medication.batch",
      "short" : "Detalhes sobre a medicação.",
      "definition" : "Informação sobre lote e validade da medicação."
    },
    {
      "id" : "Medication.batch.id",
      "path" : "Medication.batch.id",
      "max" : "0"
    },
    {
      "id" : "Medication.batch.lotNumber",
      "path" : "Medication.batch.lotNumber",
      "short" : "Lote de medicamento.",
      "definition" : "RN14: Se medicamento serializado/Datamatrix - Elemento lot do XML para grupo  IUM."
    },
    {
      "id" : "Medication.batch.expirationDate",
      "path" : "Medication.batch.expirationDate",
      "short" : "Data de validade do medicamento."
    }]
  }
}

```
