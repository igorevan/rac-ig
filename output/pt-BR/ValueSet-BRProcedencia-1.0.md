# Procedência do Contato Assistencial - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Procedência do Contato Assistencial 

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
  "id" : "BRProcedencia-1.0",
  "meta" : {
    "lastUpdated" : "2020-03-12T13:23:45.969+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRProcedencia-1.0",
  "version" : "1.0.0",
  "name" : "BRProcedencia",
  "title" : "Procedência do Contato Assistencial",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-12T13:23:45.1685886+00:00",
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
  "description" : "Classifica o serviço que encaminhou o indivíduo ou a sua iniciativa/de seu responsável na busca pelo acesso ao serviço de saúde.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRProcedencia"
    }]
  }
}

```
