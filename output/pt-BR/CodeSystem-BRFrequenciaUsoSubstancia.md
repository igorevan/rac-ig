# Frequência de Uso de Substância - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## CodeSystem: Frequência de Uso de Substância 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Frequência de Uso da Substância](ValueSet-BRFrequenciaUsoSubstancia.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRFrequenciaUsoSubstancia",
  "meta" : {
    "versionId" : "1",
    "lastUpdated" : "2020-09-20T22:59:38.544+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRFrequenciaUsoSubstancia",
  "version" : "1.0.0",
  "name" : "BRFrequenciaUsoSubstancia",
  "title" : "Frequência de Uso de Substância",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T22:59:37.2719923+00:00",
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
  "description" : "Identifica a frequência de uso da substância conforme declaração do indivíduo, de acordo com o especificado no modelo de informação do Registro de Atendimento Clínico da Resolução CIT nº 33/2018.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "nunca",
    "display" : "Nunca"
  },
  {
    "code" : "uma-ou-duas",
    "display" : "1 ou 2 vezes"
  }]
}

```
