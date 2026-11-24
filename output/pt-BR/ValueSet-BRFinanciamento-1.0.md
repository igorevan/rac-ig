# Financiamento do procedimento realizado - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Financiamento do procedimento realizado 

 **References** 

* [Financiamento](StructureDefinition-BRFinanciamento-1.0.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRFinanciamento-1.0",
  "meta" : {
    "lastUpdated" : "2020-03-12T13:10:39.310+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRFinanciamento-1.0",
  "version" : "1.0.0",
  "name" : "BRFinanciamento",
  "title" : "Financiamento do procedimento realizado",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-12T13:10:38.3145222+00:00",
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
  "description" : "Descreve o agente, instituição ou entidade responsável por custear as ações e serviços de saúde.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRFinanciamento"
    }]
  }
}

```
