# Terminologia dos medicamentos - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Terminologia dos medicamentos 

 **References** 

* [Medicamento](StructureDefinition-BRMedicamento.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRTerminologiaMedicamento",
  "meta" : {
    "lastUpdated" : "2021-12-01T13:16:09.8385573+00:00"
  },
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTerminologiaMedicamento",
  "version" : "1.0.0",
  "name" : "BRTerminologiaMedicamento",
  "title" : "Terminologia dos medicamentos",
  "status" : "active",
  "experimental" : false,
  "date" : "2021-12-01T13:16:09.8385573+00:00",
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
  "description" : "ValueSet utilizado para definir a terminologia de um dado medicamento.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRObmCATMAT"
    },
    {
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRObmEAN"
    },
    {
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRObmANVISA"
    },
    {
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRObmAMPP"
    },
    {
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRObmVMP"
    }]
  }
}

```
