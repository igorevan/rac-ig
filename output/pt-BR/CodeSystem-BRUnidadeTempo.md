# Unidade de tempo - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## CodeSystem: Unidade de tempo 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Unidade de Tempo](ValueSet-BRUnidadeTempo.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRUnidadeTempo",
  "meta" : {
    "lastUpdated" : "2022-03-22T14:53:00.0000000+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRUnidadeTempo",
  "version" : "1.0.0",
  "name" : "BRUnidadeTempo",
  "title" : "Unidade de tempo",
  "status" : "active",
  "experimental" : false,
  "date" : "2022-03-22T14:53:00.0000000+00:00",
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
  "description" : "Code System utilizado para definir a classe de unidades de tempo.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "min",
    "display" : "minuto(s)",
    "designation" : [{
      "language" : "en",
      "value" : "minute"
    }]
  },
  {
    "code" : "h",
    "display" : "hora(s)",
    "designation" : [{
      "language" : "en",
      "value" : "hour"
    }]
  },
  {
    "code" : "d",
    "display" : "dia(s)",
    "designation" : [{
      "language" : "en",
      "value" : "day"
    }]
  },
  {
    "code" : "wk",
    "display" : "semana(s)",
    "designation" : [{
      "language" : "en",
      "value" : "week"
    }]
  },
  {
    "code" : "mo",
    "display" : "mês(meses)",
    "designation" : [{
      "language" : "en",
      "value" : "month"
    }]
  },
  {
    "code" : "a",
    "display" : "ano(s)",
    "designation" : [{
      "language" : "en",
      "value" : "year"
    }]
  }]
}

```
