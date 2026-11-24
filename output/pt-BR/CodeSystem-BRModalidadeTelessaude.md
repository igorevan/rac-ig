# Modalidade de Telessaúde (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## CodeSystem: Modalidade de Telessaúde (CodeSystem) 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Modalidade de Telessaúde (ValueSet)](ValueSet-BRModalidadeTelessaude.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRModalidadeTelessaude",
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRModalidadeTelessaude",
  "version" : "1.0.0",
  "name" : "BRModalidadeTelessaude",
  "title" : "Modalidade de Telessaúde (CodeSystem)",
  "status" : "active",
  "experimental" : false,
  "date" : "2026-06-24T12:05:18.2868027+00:00",
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
  "description" : "Códigos para representação da modalidade de telessaúde realizada.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "teleconsulta",
    "display" : "Teleconsulta"
  }]
}

```
