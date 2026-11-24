# Status do atestado - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Status do atestado 

 **References** 

* [Atestado Digital](StructureDefinition-BRAtestado.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BREstadoAtestado",
  "meta" : {
    "lastUpdated" : "2023-04-13T13:17:22.715+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BREstadoAtestado",
  "version" : "1.0.0",
  "name" : "BREstadoAtestado",
  "title" : "Status do atestado",
  "status" : "active",
  "experimental" : false,
  "date" : "2023-04-13T13:17:18.5012669+00:00",
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
  "description" : "Status do atestado médico/odontológico.",
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
      }]
    }]
  }
}

```
