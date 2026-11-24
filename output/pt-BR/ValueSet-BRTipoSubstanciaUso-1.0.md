# Tipo de Substância em Uso (ValueSet) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Tipo de Substância em Uso 

 **References** 

Este conjunto de valores não é utilizado aqui; pode ser utilizado noutro local (por exemplo, especificações e/ou implementações que utilizem este conteúdo)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRTipoSubstanciaUso-1.0",
  "meta" : {
    "versionId" : "1",
    "lastUpdated" : "2020-09-20T23:01:22.994+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTipoSubstanciaUso-1.0",
  "version" : "1.0.0",
  "name" : "BRTipoSubstanciaUso",
  "title" : "Tipo de Substância em Uso",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T23:01:21.4959991+00:00",
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
  "description" : "Identifica o tipo de substância em uso conforme declaração do indivíduo, de acordo com o especificado no modelo de informação do Registro de Atendimento Clínico da Resolução CIT nº 33/2018.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoSubstanciaUso"
    }]
  }
}

```
