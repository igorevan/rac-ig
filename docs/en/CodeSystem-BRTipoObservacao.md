# Tipo de Observação (CodeSystem) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Tipo de Observação (CodeSystem) 

 
Tipo de Observação. 

This Code system is referenced in the definition of the following value sets:

* [BRTipoObservacao](ValueSet-BRTipoObservacao-1.0.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTipoObservacao",
  "meta" : {
    "lastUpdated" : "2020-03-11T18:25:29.666+00:00"
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoObservacao",
  "version" : "1.0.0-release",
  "name" : "BRTipoObservacao",
  "title" : "Tipo de Observação",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-11T18:25:50.173869+00:00",
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
  "description" : "Tipo de Observação.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "DSIA",
    "display" : "Declaração Subjetiva do Indivíudo para o Atendimento"
  },
  {
    "code" : "RECIDI",
    "display" : "Resumo da evolução clínica do indivíduo durante a internação"
  },
  {
    "code" : "DF",
    "display" : "Dados do desfecho"
  },
  {
    "code" : "IAC",
    "display" : "Informações Adicionais/Complementares"
  },
  {
    "code" : "P",
    "display" : "Peso"
  },
  {
    "code" : "A",
    "display" : "Altura"
  },
  {
    "code" : "PC",
    "display" : "Perímetro Cefálico"
  },
  {
    "code" : "CA",
    "display" : "Circunferência Abdominal"
  },
  {
    "code" : "PA",
    "display" : "Pressão Arterial"
  }]
}

```
