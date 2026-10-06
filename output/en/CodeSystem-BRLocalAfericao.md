# Local de Aferição (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Local de Aferição (CodeSystem) 

This Code system is referenced in the definition of the following value sets:

* [Local de Aferição](ValueSet-BRLocalAfericao-1.0.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRLocalAfericao",
  "meta" : {
    "lastUpdated" : "2020-03-11T18:15:18.190+00:00"
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRLocalAfericao",
  "version" : "1.0.0-release",
  "name" : "BRLocalAfericao",
  "title" : "Local de Aferição",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-11T18:15:38.6898126+00:00",
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
  "description" : "Identifica a parte do corpo utilizada para realizar uma mensuração ou aferição.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "1",
    "display" : "Braço direito"
  },
  {
    "code" : "2",
    "display" : "Braço esquerdo"
  },
  {
    "code" : "3",
    "display" : "Coxa direita"
  },
  {
    "code" : "4",
    "display" : "Coxa esquerda"
  },
  {
    "code" : "5",
    "display" : "Pulso direito"
  },
  {
    "code" : "6",
    "display" : "Pulso esquerdo"
  },
  {
    "code" : "7",
    "display" : "Tornozelo direito"
  },
  {
    "code" : "8",
    "display" : "Tornozelo esquerdo"
  },
  {
    "code" : "9",
    "display" : "Dedo da mão"
  },
  {
    "code" : "10",
    "display" : "Dedo do pé"
  }]
}

```
