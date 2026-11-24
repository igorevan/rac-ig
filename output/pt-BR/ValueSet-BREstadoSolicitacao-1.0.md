# Estado da Solicitação - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Estado da Solicitação 

 **References** 

* [Plano de Cuidados](StructureDefinition-BRPlanoCuidados-1.0.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BREstadoSolicitacao-1.0",
  "language" : "en",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BREstadoSolicitacao-1.0",
  "version" : "1.0.0",
  "name" : "BREstadoSolicitacao",
  "title" : "Estado da Solicitação",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T20:51:00.5465258+00:00",
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
  "description" : "Estado da solicitação.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://hl7.org/fhir/request-status",
      "concept" : [{
        "code" : "active",
        "display" : "Active",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Ativo"
        }]
      },
      {
        "code" : "entered-in-error",
        "display" : "Entered in Error",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Cancelada por informação errada"
        }]
      }]
    }]
  }
}

```
