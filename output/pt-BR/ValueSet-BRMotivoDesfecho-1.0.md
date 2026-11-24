# Motivo do desfecho do Contato Assistencial - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Motivo do desfecho do Contato assistencial 

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
  "id" : "BRMotivoDesfecho-1.0",
  "meta" : {
    "lastUpdated" : "2020-03-12T13:18:05.304+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRMotivoDesfecho-1.0",
  "version" : "1.0.0",
  "name" : "BRMotivoDesfecho",
  "title" : "Motivo do desfecho do Contato assistencial",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-12T13:18:04.0945614+00:00",
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
  "description" : "ValueSet utilizado para classificar o motivo de conclusão total ou parcial do contato assistencial.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRMotivoDesfecho"
    }]
  }
}

```
