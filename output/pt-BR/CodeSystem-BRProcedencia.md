# Procedência - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## CodeSystem: Procedência 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Procedência do Contato Assistencial](ValueSet-BRProcedencia-1.0.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRProcedencia",
  "meta" : {
    "lastUpdated" : "2020-04-17T14:46:11.153+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRProcedencia",
  "version" : "1.0.0",
  "name" : "BRProcedencia",
  "title" : "Procedência",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-04-17T14:46:08.158574+00:00",
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
  "description" : "Identifica o serviço que encaminhou o indivíduo ou a sua iniciativa/de seu responsável na busca pelo acesso ao serviço de saúde.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "09",
    "display" : "Demanda espontânea"
  },
  {
    "code" : "10",
    "display" : "Ordem Judicial"
  },
  {
    "code" : "11",
    "display" : "Retorno"
  },
  {
    "code" : "12",
    "display" : "Demanda referenciada"
  },
  {
    "code" : "99",
    "display" : "Informação ausente no modelo de origem"
  }]
}

```
