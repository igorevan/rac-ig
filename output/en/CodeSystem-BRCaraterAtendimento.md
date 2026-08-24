# Caráter de Atendimento - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Caráter de Atendimento 

 
Terminologia que classifica a prioridade de realização de um Contato Assistencial. 

This Code system is referenced in the definition of the following value sets:

* [Caráter de atendimento do Contato Assistencial](ValueSet-BRCaraterAtendimento-1.0.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRCaraterAtendimento",
  "meta" : {
    "lastUpdated" : "2020-03-11T11:56:57.326+00:00"
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRCaraterAtendimento",
  "version" : "1.0.0-release",
  "name" : "BRCaraterAtendimento",
  "title" : "Caráter de Atendimento",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-11T11:57:17.2973841+00:00",
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
  "description" : "Terminologia que classifica a prioridade de realização de um Contato Assistencial.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "concept" : [{
    "code" : "01",
    "display" : "Eletivo"
  },
  {
    "code" : "02",
    "display" : "Urgência"
  },
  {
    "code" : "03",
    "display" : "Consulta agendada"
  },
  {
    "code" : "04",
    "display" : "Consulta agendada programada: cuidado continuado"
  },
  {
    "code" : "05",
    "display" : "Demanda espontânea (DE): consulta no dia"
  },
  {
    "code" : "06",
    "display" : "Demanda espontânea (DE): atendimento de urgência"
  },
  {
    "code" : "99",
    "display" : "Sem registro no modelo de informação de origem"
  }]
}

```
