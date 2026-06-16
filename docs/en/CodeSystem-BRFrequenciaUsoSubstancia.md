# Frequência de Uso de Substância - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Frequência de Uso de Substância 

 
Identifica a frequência de uso da substância conforme declaração do indivíduo, de acordo com o especificado no modelo de informação do Registro de Atendimento Clínico da Resolução CIT nº 33/2018. 

This Code system is referenced in the definition of the following value sets:

* [BRFrequenciaUsoSubstancia](ValueSet-BRFrequenciaUsoSubstancia.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



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
  "extension" : [{
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-wg",
    "valueCode" : "ehr"
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-fmm",
    "valueInteger" : 1,
    "_valueInteger" : {
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-conformance-derivedFrom",
        "valueCanonical" : "https://fhir.saude.gov.br/fhir/r4/rac/1.0.0/ImplementationGuide/br.gov.saude.rac.fhir"
      }]
    }
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
    "valueCode" : "normative",
    "_valueCode" : {
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-conformance-derivedFrom",
        "valueCanonical" : "https://fhir.saude.gov.br/fhir/r4/rac/1.0.0/ImplementationGuide/br.gov.saude.rac.fhir"
      }]
    }
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
    "valueCode" : "4.0.1"
  }],
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRFrequenciaUsoSubstancia",
  "version" : "1.0.0-release",
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
