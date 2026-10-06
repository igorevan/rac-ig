# Estado da Solicitação de Medicamento - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## ValueSet: Estado da Solicitação de Medicamento 

 **References** 

* [Medicamento](StructureDefinition-BRMedicamento.md)

### Logical Definition (CLD)

 

### Expansion

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BREstadoSolicitacaoMedicamento-1.0",
  "language" : "en",
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
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BREstadoSolicitacaoMedicamento-1.0",
  "version" : "1.0.0-release",
  "name" : "BREstadoSolicitacaoMedicamento",
  "title" : "Estado da Solicitação de Medicamento",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T20:58:15.9226123+00:00",
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
  "description" : "Estado da Solicitação de Medicamento",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : true,
  "compose" : {
    "include" : [{
      "system" : "http://hl7.org/fhir/CodeSystem/medicationrequest-status",
      "concept" : [{
        "code" : "active",
        "display" : "Active",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Ativo"
        }]
      },
      {
        "code" : "completed",
        "display" : "Completed",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Completado"
        }]
      },
      {
        "code" : "entered-in-error",
        "display" : "Entered in Error",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Entrada com erro"
        }]
      },
      {
        "code" : "draft",
        "display" : "Draft",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Pretendido"
        }]
      },
      {
        "code" : "on-hold",
        "display" : "On Hold",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Em pausa"
        }]
      },
      {
        "code" : "unknown",
        "display" : "Unknown",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Desconhecida"
        }]
      },
      {
        "code" : "cancelled",
        "display" : "Cancelled",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Não realizado"
        }]
      }]
    }]
  }
}

```
