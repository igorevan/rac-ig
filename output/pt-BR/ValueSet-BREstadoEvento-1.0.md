# Estado do Evento - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Estado do Evento 

 **References** 

* [Procedimento Realizado](StructureDefinition-BRProcedimentoRealizado-1.0.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BREstadoEvento-1.0",
  "language" : "en",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BREstadoEvento-1.0",
  "version" : "1.0.0",
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
