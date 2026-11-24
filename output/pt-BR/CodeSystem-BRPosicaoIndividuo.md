# Posição do Indivíduo (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## CodeSystem: Posição do Indivíduo (CodeSystem) 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Posição do Indivíduo](ValueSet-BRPosicaoIndividuo.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRPosicaoIndividuo",
  "meta" : {
    "lastUpdated" : "2020-03-11T18:19:54.794+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRPosicaoIndividuo",
  "version" : "1.0.0",
  "name" : "BRPosicaoIndividuo",
  "title" : "Posição do Indivíduo",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-11T18:20:15.3085069+00:00",
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
  "description" : "Identifica a posição de um indivíduo em um determinado contexto.",
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
    "display" : "Em pé"
  },
  {
    "code" : "2",
    "display" : "Sentado"
  },
  {
    "code" : "3",
    "display" : "Reclinado"
  },
  {
    "code" : "4",
    "display" : "Deitado"
  },
  {
    "code" : "5",
    "display" : "Deitado com inclinação para esquerda"
  }]
}

```
