# Turno do dia (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## CodeSystem: Turno do dia (CodeSystem) 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Turno do dia](ValueSet-BRTurno.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTurno",
  "meta" : {
    "lastUpdated" : "2021-12-01T13:16:09.8385573+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTurno",
  "version" : "1.0.0",
  "name" : "BRTurno",
  "title" : "Turno do dia",
  "status" : "active",
  "experimental" : false,
  "date" : "2021-12-01T13:16:09.8385573+00:00",
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
  "description" : "Code System utilizado para definir o turno de um dia.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "1",
    "display" : "Manhã"
  },
  {
    "code" : "2",
    "display" : "Tarde"
  },
  {
    "code" : "3",
    "display" : "Noite"
  }]
}

```
