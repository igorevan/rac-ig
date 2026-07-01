# Classificação do papel de um problema e diagnóstico (ValueSet) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## ValueSet: Classificação do papel de um problema e diagnóstico 

 
Tradução para o português do brasil da classificação do papel de um problema/diagnóstico. 

 **References** 

* [Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md)

### Logical Definition (CLD)

 

### Expansion

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRPapelProblemaDiagnostico",
  "meta" : {
    "lastUpdated" : "2020-03-11T19:14:51.806+00:00"
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
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRPapelProblemaDiagnostico",
  "version" : "1.0.0-release",
  "name" : "BRPapelProblemaDiagnostico",
  "title" : "Classificação do papel de um problema e diagnóstico",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-11T19:15:12.2909517+00:00",
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
  "description" : "Tradução para o português do brasil da classificação do papel de um problema/diagnóstico.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRPapelProblemaDiagnostico"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/diagnosis-role",
      "concept" : [{
        "code" : "AD",
        "display" : "Admission diagnosis",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Diagnóstico presente na admissão"
        }]
      },
      {
        "code" : "DD",
        "display" : "Discharge diagnosis",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Diagnóstico de alta"
        }]
      },
      {
        "code" : "CC",
        "display" : "Chief complaint",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Queixa principal."
        }]
      },
      {
        "code" : "CM",
        "display" : "Comorbidity diagnosis",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Diagnóstico de comorbidade"
        }]
      },
      {
        "code" : "pre-op",
        "display" : "pre-op diagnosis",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Diagnóstico pré-operatório"
        }]
      },
      {
        "code" : "post-op",
        "display" : "post-op diagnosis",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Diagnóstico pós-operatório"
        }]
      },
      {
        "code" : "billing",
        "display" : "Billing",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Faturamento"
        }]
      }]
    }]
  }
}

```
