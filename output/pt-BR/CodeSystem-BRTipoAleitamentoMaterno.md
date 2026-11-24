# Tipo de Aleitamento Materno (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## CodeSystem: Tipo de Aleitamento Materno (CodeSystem) 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Tipo de Aleitamento Materno](ValueSet-BRTipoAleitamentoMaterno-1.0.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTipoAleitamentoMaterno",
  "meta" : {
    "versionId" : "1",
    "lastUpdated" : "2020-09-20T22:50:41.993+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoAleitamentoMaterno",
  "version" : "1.0.0",
  "name" : "BRTipoAleitamentoMaterno",
  "title" : "Tipo de Aleitamento Materno",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T22:50:40.2386423+00:00",
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
  "description" : "Classifica o tipo de aleitamento materno realizado a uma criança.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "exclusivo",
    "display" : "Exclusivo"
  },
  {
    "code" : "predominante",
    "display" : "Predominante"
  },
  {
    "code" : "complementado",
    "display" : "Complementado"
  },
  {
    "code" : "inexistente",
    "display" : "Inexistente"
  }]
}

```
