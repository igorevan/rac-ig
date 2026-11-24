# Tipo de atestado - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Tipo de atestado 

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
  "id" : "BRTipoAtestado",
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTipoAtestado",
  "version" : "1.0.0",
  "name" : "BRTipoAtestado",
  "title" : "Tipo de atestado",
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
  "description" : "Tipo de atestado dentro das categorias médico/odontológico",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoDocumento",
      "concept" : [{
        "code" : "ATM"
      }]
    }]
  }
}

```
