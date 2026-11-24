# Responsabilidade no Contato Assistencial (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## CodeSystem: Responsabilidade no Contato Assistencial (CodeSystem) 

Este sistema de códigos é referenciado na definição dos seguintes conjuntos de valores:

* [Reponsabilidade no Contato Assistencial](ValueSet-BRResponsabilidadeParticipante-1.0.md)

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRResponsabilidadeParticipante",
  "meta" : {
    "lastUpdated" : "2020-03-11T18:20:28.411+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRResponsabilidadeParticipante",
  "version" : "1.0.0",
  "name" : "BRResponsabilidadeParticipante",
  "title" : "Responsabilidade no Contato Assistencial",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-11T18:20:48.9276301+00:00",
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
  "description" : "Classifica o tipo de responsabilidade de indivíduos ou profissionais no Contato Assisntecial.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "solicitante",
    "display" : "Profissional que solicitou o Contato Assistencial"
  },
  {
    "code" : "autorizador",
    "display" : "Profissional que autorizou a realização do Contato Assistencial"
  },
  {
    "code" : "admissao",
    "display" : "Profissional que admitiu do indivíduo no Contato Assistencial"
  },
  {
    "code" : "alta",
    "display" : "Profissional que realizou a alta do indivíduo no Contato Assistencial"
  },
  {
    "code" : "atendimento",
    "display" : "Profissional responsável pelo atendimento clínico Contato Assistencial"
  }]
}

```
