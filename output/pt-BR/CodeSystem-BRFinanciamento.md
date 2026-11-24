# Financiamento (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## CodeSystem: Financiamento (CodeSystem) 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Financiamento do procedimento realizado](ValueSet-BRFinanciamento-1.0.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRFinanciamento",
  "meta" : {
    "lastUpdated" : "2020-03-11T18:12:26.041+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRFinanciamento",
  "version" : "1.0.0",
  "name" : "BRFinanciamento",
  "title" : "Financiamento",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-11T18:12:46.5570008+00:00",
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
  "description" : "Terminologia que descreve o agente, instituição ou entidade responsável por custear as ações e serviços de saúde.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "01",
    "display" : "Federal SUS"
  },
  {
    "code" : "02",
    "display" : "Plano de Saúde Público"
  },
  {
    "code" : "03",
    "display" : "Plano de Saúde Privado"
  },
  {
    "code" : "04",
    "display" : "Particular"
  },
  {
    "code" : "05",
    "display" : "Gratuidade"
  },
  {
    "code" : "06",
    "display" : "Estadual SUS"
  },
  {
    "code" : "07",
    "display" : "Municipal SUS"
  },
  {
    "code" : "08",
    "display" : "Programas e Projetos Federais"
  }]
}

```
