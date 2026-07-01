# Tipo de Aleitamento Materno (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Tipo de Aleitamento Materno (CodeSystem) 

 
Classifica o tipo de aleitamento materno realizado a uma criança. 

This Code system is referenced in the definition of the following value sets:

* [BRTipoAleitamentoMaterno](ValueSet-BRTipoAleitamentoMaterno-1.0.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTipoAleitamentoMaterno",
  "meta" : {
    "versionId" : "1",
    "lastUpdated" : "2020-09-20T22:50:41.993+00:00"
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoAleitamentoMaterno",
  "version" : "1.0.0-release",
  "name" : "BRTipoAleitamentoMaterno",
  "title" : "Tipo de Aleitamento Materno",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T22:50:40.2386423+00:00",
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
  "description" : "Classifica o tipo de aleitamento materno realizado a uma criança.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "exclusivo",
    "display" : "Exclusivo"
  },
  {
    "code" : "predominante",
    "display" : "Predominante"
  },
  {
    "code" : "complementado",
    "display" : "Complementado"
  },
  {
    "code" : "inexistente",
    "display" : "Inexistente"
  }]
}

```
