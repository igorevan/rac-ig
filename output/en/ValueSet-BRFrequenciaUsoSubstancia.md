# Frequência de Uso da Substância - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## ValueSet: Frequência de Uso da Substância 

 **References** 

* [Medida Observada](StructureDefinition-BRMedidaObservada.md)

### Definição lógica (CLD)

 

### Expansion

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRFrequenciaUsoSubstancia",
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
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRFrequenciaUsoSubstancia",
  "version" : "1.0.0-release",
  "name" : "BRFrequenciaUsoSubstancia",
  "title" : "Frequência de Uso da Substância",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T23:02:23.9723544+00:00",
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
  "description" : "Identifica a frequência de uso da substância em uso conforme declaração do indivíduo.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-GTSAbbreviation",
      "concept" : [{
        "code" : "MO",
        "display" : "monthly",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Mensalmente"
        }]
      },
      {
        "code" : "WK",
        "display" : "weekly",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Semanalmente"
        }]
      },
      {
        "code" : "QD",
        "display" : "QD",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Diariamente"
        }]
      }]
    },
    {
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRFrequenciaUsoSubstancia"
    }]
  }
}

```
