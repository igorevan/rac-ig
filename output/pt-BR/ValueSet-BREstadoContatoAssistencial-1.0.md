# Estado do Contato Assistencial - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Estado do Contato Assistencial 

 **References** 

* [Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BREstadoContatoAssistencial-1.0",
  "language" : "en",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BREstadoContatoAssistencial-1.0",
  "version" : "1.0.0",
  "name" : "BREstadoContatoAssistencial",
  "title" : "Estado do Contato Assistencial",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-04-07T21:01:35.632661+00:00",
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
  "description" : "Classifica o estado de um Contato Assistencial.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://hl7.org/fhir/encounter-status",
      "concept" : [{
        "code" : "finished",
        "display" : "Finished",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Contato Assistencial finalizado ou concluído"
        }]
      },
      {
        "code" : "entered-in-error",
        "display" : "Entered in Error",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Contato Assistencial anulado por informação errada"
        }]
      }]
    }]
  }
}

```
