# Alérgenos - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Alérgenos 

 **References** 

* [Alergia ou Reação Adversa](StructureDefinition-BRAlergiaReacaoAdversa-1.0.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRAlergenos-1.0",
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRAlergenos-1.0",
  "version" : "1.0.0",
  "name" : "BRAlergenos",
  "title" : "Alérgenos",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T20:36:53.3154683+00:00",
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
  "description" : "Descreve o agente capaz de causar alergia ou reação adversa em seres humanos.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRAlergenosCBARA"
    },
    {
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRImunobiologico"
    },
    {
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRMedicamento"
    }]
  }
}

```
