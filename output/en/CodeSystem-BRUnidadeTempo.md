# Unidade de tempo - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Unidade de tempo 

This Code system is referenced in the definition of the following value sets:

* [Unidade de Tempo](ValueSet-BRUnidadeTempo.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRUnidadeTempo",
  "meta" : {
    "lastUpdated" : "2022-03-22T14:53:00.0000000+00:00"
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRUnidadeTempo",
  "version" : "1.0.0-release",
  "name" : "BRUnidadeTempo",
  "title" : "Unidade de tempo",
  "status" : "active",
  "experimental" : false,
  "date" : "2022-03-22T14:53:00.0000000+00:00",
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
  "description" : "Code System utilizado para definir a classe de unidades de tempo.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "min",
    "display" : "minuto(s)",
    "designation" : [{
      "language" : "en",
      "value" : "minute"
    }]
  },
  {
    "code" : "h",
    "display" : "hora(s)",
    "designation" : [{
      "language" : "en",
      "value" : "hour"
    }]
  },
  {
    "code" : "d",
    "display" : "dia(s)",
    "designation" : [{
      "language" : "en",
      "value" : "day"
    }]
  },
  {
    "code" : "wk",
    "display" : "semana(s)",
    "designation" : [{
      "language" : "en",
      "value" : "week"
    }]
  },
  {
    "code" : "mo",
    "display" : "mês(meses)",
    "designation" : [{
      "language" : "en",
      "value" : "month"
    }]
  },
  {
    "code" : "a",
    "display" : "ano(s)",
    "designation" : [{
      "language" : "en",
      "value" : "year"
    }]
  }]
}

```
