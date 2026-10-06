# Plano de Cuidados - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## Resource Profile: Plano de Cuidados 

**Usos:**

* Refere a este Perfil: [Registro de Atendimento Clínico](StructureDefinition-BRRegistroAtendimentoClinico.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/br.gov.saude.rac.fhir|current/StructureDefinition/StructureDefinition-BRPlanoCuidados-1.0.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-BRPlanoCuidados-1.0.csv), [Excel](../StructureDefinition-BRPlanoCuidados-1.0.xlsx), [Schematron](../StructureDefinition-BRPlanoCuidados-1.0.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "BRPlanoCuidados-1.0",
  "meta" : {
    "lastUpdated" : "2020-09-20T20:51:45.157+00:00"
  },
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
  "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRPlanoCuidados-1.0",
  "version" : "1.0.0-release",
  "name" : "BRPlanoCuidados",
  "title" : "Plano de Cuidados",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T20:51:44.9643607+00:00",
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
  "description" : "Descreve o plano de cuidados, instruções e recomendações.",
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
  "type" : "CarePlan",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/CarePlan",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "CarePlan",
      "path" : "CarePlan",
      "short" : "Plano de cuidados de paciente ou grupo",
      "definition" : "Descreve o plano de um ou mais profissionais para o cuidado de um paciente em particular, grupo ou comunidade em um período, possivelmente limitado ao cuidado de uma condição específica ou conjunto de condoções.",
      "mustSupport" : true
    },
    {
      "id" : "CarePlan.identifier",
      "path" : "CarePlan.identifier",
      "max" : "0"
    },
    {
      "id" : "CarePlan.instantiatesCanonical",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "CarePlan.instantiatesCanonical",
      "max" : "0"
    },
    {
      "id" : "CarePlan.instantiatesUri",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "CarePlan.instantiatesUri",
      "max" : "0"
    },
    {
      "id" : "CarePlan.basedOn",
      "path" : "CarePlan.basedOn",
      "max" : "0"
    },
    {
      "id" : "CarePlan.replaces",
      "path" : "CarePlan.replaces",
      "max" : "0"
    },
    {
      "id" : "CarePlan.partOf",
      "path" : "CarePlan.partOf",
      "max" : "0"
    },
    {
      "id" : "CarePlan.status",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "CarePlan.status",
      "short" : "Estado do Plano de Cuidados",
      "definition" : "Indica se o plano está em curso, se representa intenções guturas ou é um registro de histórico.\nactive: Ativo\nentered-in-error: Cancelado por informação errada",
      "mustSupport" : true,
      "binding" : {
        "strength" : "required",
        "description" : "Estado da Solicitação",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BREstadoSolicitacao-1.0"
      }
    },
    {
      "id" : "CarePlan.intent",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "CarePlan.intent",
      "short" : "Intenção do Plano de Cuidados",
      "definition" : "Indica o nível de autoridade/intenção associado ao plano de cuidados e onde ele se encaixa no fluxo de trabalho.",
      "fixedCode" : "plan",
      "mustSupport" : true,
      "binding" : {
        "strength" : "required",
        "description" : "Intenção do Plano de Cuidados"
      }
    },
    {
      "id" : "CarePlan.category",
      "path" : "CarePlan.category",
      "max" : "0"
    },
    {
      "id" : "CarePlan.title",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "CarePlan.title",
      "max" : "0"
    },
    {
      "id" : "CarePlan.description",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "CarePlan.description",
      "short" : "Descrição do Plano de Cuidados, Instruções e Recomendações",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "CarePlan.subject",
      "path" : "CarePlan.subject",
      "short" : "Indivíduo do Plano de Cuidados",
      "definition" : "Pessoa ao qual o plano de cuidados se refere.",
      "type" : [{
        "code" : "Reference",
        "targetProfile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0"]
      }],
      "mustSupport" : true
    },
    {
      "id" : "CarePlan.subject.extension",
      "path" : "CarePlan.subject.extension",
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
      "id" : "CarePlan.subject.extension:unidentifiedPatient",
      "path" : "CarePlan.subject.extension",
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
      "id" : "CarePlan.subject.extension:unidentifiedPatient.extension",
      "path" : "CarePlan.subject.extension.extension",
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
      "id" : "CarePlan.subject.extension:unidentifiedPatient.extension:gender",
      "path" : "CarePlan.subject.extension.extension",
      "sliceName" : "gender",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "CarePlan.subject.extension:unidentifiedPatient.extension:birthYear",
      "path" : "CarePlan.subject.extension.extension",
      "sliceName" : "birthYear",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "CarePlan.subject.extension:unidentifiedPatient.extension:reason",
      "path" : "CarePlan.subject.extension.extension",
      "sliceName" : "reason",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "CarePlan.subject.reference",
      "path" : "CarePlan.subject.reference",
      "max" : "0"
    },
    {
      "id" : "CarePlan.subject.type",
      "path" : "CarePlan.subject.type",
      "max" : "0"
    },
    {
      "id" : "CarePlan.subject.identifier",
      "path" : "CarePlan.subject.identifier",
      "min" : 1
    },
    {
      "id" : "CarePlan.subject.identifier.use",
      "path" : "CarePlan.subject.identifier.use",
      "max" : "0"
    },
    {
      "id" : "CarePlan.subject.identifier.type",
      "path" : "CarePlan.subject.identifier.type",
      "max" : "0"
    },
    {
      "id" : "CarePlan.subject.identifier.system",
      "path" : "CarePlan.subject.identifier.system",
      "min" : 1
    },
    {
      "id" : "CarePlan.subject.identifier.value",
      "path" : "CarePlan.subject.identifier.value",
      "min" : 1
    },
    {
      "id" : "CarePlan.subject.identifier.period",
      "path" : "CarePlan.subject.identifier.period",
      "max" : "0"
    },
    {
      "id" : "CarePlan.subject.identifier.assigner",
      "path" : "CarePlan.subject.identifier.assigner",
      "max" : "0"
    },
    {
      "id" : "CarePlan.subject.display",
      "path" : "CarePlan.subject.display",
      "max" : "0"
    },
    {
      "id" : "CarePlan.encounter",
      "path" : "CarePlan.encounter",
      "max" : "0"
    },
    {
      "id" : "CarePlan.period",
      "path" : "CarePlan.period",
      "max" : "0"
    },
    {
      "id" : "CarePlan.created",
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
        "valueCode" : "normative"
      },
      {
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
        "valueCode" : "4.0.0"
      }],
      "path" : "CarePlan.created",
      "max" : "0"
    },
    {
      "id" : "CarePlan.author",
      "path" : "CarePlan.author",
      "max" : "0"
    },
    {
      "id" : "CarePlan.contributor",
      "path" : "CarePlan.contributor",
      "max" : "0"
    },
    {
      "id" : "CarePlan.careTeam",
      "path" : "CarePlan.careTeam",
      "max" : "0"
    },
    {
      "id" : "CarePlan.addresses",
      "path" : "CarePlan.addresses",
      "max" : "0"
    },
    {
      "id" : "CarePlan.supportingInfo",
      "path" : "CarePlan.supportingInfo",
      "max" : "0"
    },
    {
      "id" : "CarePlan.goal",
      "path" : "CarePlan.goal",
      "max" : "0"
    },
    {
      "id" : "CarePlan.activity",
      "path" : "CarePlan.activity",
      "max" : "0"
    },
    {
      "id" : "CarePlan.note",
      "path" : "CarePlan.note",
      "max" : "0"
    }]
  }
}

```
