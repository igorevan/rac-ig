# Tipo de Observação (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## CodeSystem: Tipo de Observação (CodeSystem) 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Tipo de Observação](ValueSet-BRTipoObservacao-1.0.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTipoObservacao",
  "meta" : {
    "lastUpdated" : "2020-03-11T18:25:29.666+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoObservacao",
  "version" : "1.0.0",
  "name" : "BRTipoObservacao",
  "title" : "Tipo de Observação",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-11T18:25:50.173869+00:00",
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
  "description" : "Tipo de Observação.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "DSIA",
    "display" : "Declaração Subjetiva do Indivíudo para o Atendimento"
  },
  {
    "code" : "RECIDI",
    "display" : "Resumo da evolução clínica do indivíduo durante a internação"
  },
  {
    "code" : "DF",
    "display" : "Dados do desfecho"
  },
  {
    "code" : "IAC",
    "display" : "Informações Adicionais/Complementares"
  },
  {
    "code" : "P",
    "display" : "Peso"
  },
  {
    "code" : "A",
    "display" : "Altura"
  },
  {
    "code" : "PC",
    "display" : "Perímetro Cefálico"
  },
  {
    "code" : "CA",
    "display" : "Circunferência Abdominal"
  },
  {
    "code" : "PA",
    "display" : "Pressão Arterial"
  }]
}

```
