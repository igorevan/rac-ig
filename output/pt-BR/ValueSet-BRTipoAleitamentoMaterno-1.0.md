# Tipo de Aleitamento Materno (ValueSet) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Tipo de Aleitamento Materno 

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
  "id" : "BRTipoAleitamentoMaterno-1.0",
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTipoAleitamentoMaterno-1.0",
  "version" : "1.0.0",
  "name" : "BRTipoAleitamentoMaterno",
  "title" : "Tipo de Aleitamento Materno",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-12T14:51:30.2531733+00:00",
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
  "description" : "Definição do tipo de aleitamento materno realizado a uma criança.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoAleitamentoMaterno"
    }]
  }
}

```
