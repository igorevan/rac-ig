# Categoria do Diagnóstico (ValueSet) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Categoria do Diagnóstico 

 **References** 

* [CID10 Avaliado](StructureDefinition-BRCID10Avaliado-1.0.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRCategoriaDiagnostico",
  "meta" : {
    "lastUpdated" : "2022-05-19T11:10:40.0457007+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRCategoriaDiagnostico",
  "version" : "1.0.0",
  "name" : "BRCategoriaDiagnostico",
  "title" : "Categoria do Diagnóstico",
  "status" : "active",
  "experimental" : false,
  "date" : "2022-05-19T11:10:40.0457007+00:00",
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
  "description" : "ValueSet utilizado para definir o tipo de categoria do diagnóstico realizado.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRCategoriaDiagnostico"
    }]
  }
}

```
