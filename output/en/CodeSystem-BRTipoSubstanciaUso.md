# Tipo de Substância em Uso (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Tipo de Substância em Uso (CodeSystem) 

This Code system is referenced in the definition of the following value sets:

* [Tipo de Substância em Uso](ValueSet-BRTipoSubstanciaUso-1.0.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTipoSubstanciaUso",
  "meta" : {
    "versionId" : "1",
    "lastUpdated" : "2020-09-20T23:04:32.536+00:00"
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
        "valueCanonical" : "https://fhir.saude.gov.br/rac/ImplementationGuide/br.gov.saude.rac.fhir"
      }]
    }
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-standards-status",
    "valueCode" : "normative",
    "_valueCode" : {
      "extension" : [{
        "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-conformance-derivedFrom",
        "valueCanonical" : "https://fhir.saude.gov.br/rac/ImplementationGuide/br.gov.saude.rac.fhir"
      }]
    }
  },
  {
    "url" : "http://hl7.org/fhir/StructureDefinition/structuredefinition-normative-version",
    "valueCode" : "4.0.1"
  }],
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoSubstanciaUso",
  "version" : "1.0.0-release",
  "name" : "BRTipoSubstanciaUso",
  "title" : "Tipo de Substância em Uso",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T23:04:30.8771699+00:00",
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
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "deriv-tabaco",
    "display" : "Derivados do Tabaco"
  },
  {
    "code" : "alcool",
    "display" : "Bebidas Alcóolicas"
  },
  {
    "code" : "maconha",
    "display" : "Maconha"
  },
  {
    "code" : "cocaina",
    "display" : "Cocaína"
  },
  {
    "code" : "crack",
    "display" : "Crack"
  },
  {
    "code" : "anfetamina",
    "display" : "Anfetaminas ou Êxtase"
  },
  {
    "code" : "inalante",
    "display" : "Inalantes"
  },
  {
    "code" : "hipno-seda",
    "display" : "Hipnóticos ou Sedativos"
  },
  {
    "code" : "alucinogeno",
    "display" : "Alucinógenos"
  },
  {
    "code" : "opio",
    "display" : "Opióides ou Opiáceos"
  }]
}

```
