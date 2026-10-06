# Estado do Evento - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## ValueSet: Estado do Evento 

 **References** 

* [Procedimento Realizado](StructureDefinition-BRProcedimentoRealizado-1.0.md)

### Logical Definition (CLD)

 

### Expansion

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BREstadoEvento-1.0",
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
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BREstadoEvento-1.0",
  "version" : "1.0.0-release",
  "name" : "BREstadoEvento",
  "title" : "Estado do Evento",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-04-07T12:14:07.8417018+00:00",
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
  "description" : "Identificação do estado de um evento.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://hl7.org/fhir/event-status",
      "concept" : [{
        "code" : "preparation",
        "display" : "Preparation",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Pré-procedimento"
        }]
      },
      {
        "code" : "in-progress",
        "display" : "In Progress",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Em andamento"
        }]
      },
      {
        "code" : "not-done",
        "display" : "Not Done",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Não Realizado"
        }]
      },
      {
        "code" : "on-hold",
        "display" : "On Hold",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Suspenso"
        }]
      },
      {
        "code" : "stopped",
        "display" : "Stopped",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Cancelado"
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
        "code" : "unknown",
        "display" : "Unknown",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Desconhecido"
        }]
      },
      {
        "code" : "entered-in-error",
        "display" : "Entered in Error",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Entrada com erro"
        }]
      }]
    }]
  }
}

```
