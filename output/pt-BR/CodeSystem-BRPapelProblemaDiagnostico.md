# Classificação do papel de um problema e diagnóstico (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## CodeSystem: Classificação do papel de um problema e diagnóstico (CodeSystem) 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Classificação do papel de um problema e diagnóstico](ValueSet-BRPapelProblemaDiagnostico.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRPapelProblemaDiagnostico",
  "meta" : {
    "lastUpdated" : "2020-03-11T18:16:07.800+00:00"
  },
  "language" : "en",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRPapelProblemaDiagnostico",
  "version" : "1.0.0",
  "name" : "BRPapelProblemaDiagnostico",
  "title" : "Classificação do papel de um problema e diagnóstico",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-11T18:16:28.3110021+00:00",
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
  "description" : "Classificação do papel de um problema/diagnóstico.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "NAD",
    "display" : "Diagnosis not present on admission",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Diagnóstico não presente na admissão"
    }]
  },
  {
    "code" : "UNK",
    "display" : "Unknown",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Desconhecido"
    }]
  }]
}

```
