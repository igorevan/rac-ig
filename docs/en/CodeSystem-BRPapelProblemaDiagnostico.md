# Classificação do papel de um problema e diagnóstico (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Classificação do papel de um problema e diagnóstico (CodeSystem) 

 
Classificação do papel de um problema/diagnóstico. 

This Code system is referenced in the definition of the following value sets:

* [BRPapelProblemaDiagnostico](ValueSet-BRPapelProblemaDiagnostico.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRPapelProblemaDiagnostico",
  "meta" : {
    "lastUpdated" : "2020-03-11T18:16:07.800+00:00"
  },
  "language" : "en",
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRPapelProblemaDiagnostico",
  "version" : "1.0.0-release",
  "name" : "BRPapelProblemaDiagnostico",
  "title" : "Classificação do papel de um problema e diagnóstico",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-11T18:16:28.3110021+00:00",
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
  "description" : "Classificação do papel de um problema/diagnóstico.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "NAD",
    "display" : "Diagnosis not present on admission",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Diagnóstico não presente na admissão"
    }]
  },
  {
    "code" : "UNK",
    "display" : "Unknown",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Desconhecido"
    }]
  }]
}

```
