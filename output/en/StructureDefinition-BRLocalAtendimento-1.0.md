# Local de Atendimento - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## Resource Profile: Local de Atendimento 

 
Uma referência genérica aos locais onde um Contato Assistencial pode acontecer. 

**Usos:**

* Refere a este Perfil: [Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/br.gov.saude.rac.fhir|current/StructureDefinition/StructureDefinition-BRLocalAtendimento-1.0.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-BRLocalAtendimento-1.0.csv), [Excel](../StructureDefinition-BRLocalAtendimento-1.0.xlsx), [Schematron](../StructureDefinition-BRLocalAtendimento-1.0.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "BRLocalAtendimento-1.0",
  "meta" : {
    "lastUpdated" : "2020-03-11T01:07:07.432+00:00"
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
  "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRLocalAtendimento-1.0",
  "version" : "1.0.0-release",
  "name" : "BRLocalAtendimento",
  "title" : "Local de Atendimento",
  "status" : "active",
  "date" : "2020-03-11T01:07:05.6772929+00:00",
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
  "description" : "Uma referência genérica aos locais onde um Contato Assistencial pode acontecer.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  },
  {
    "identity" : "w5",
    "uri" : "http://hl7.org/fhir/fivews",
    "name" : "FiveWs Pattern Mapping"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Location",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Location",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Location",
      "path" : "Location",
      "short" : "Local de Atendimento",
      "definition" : "Uma referência genérica aos locais onde um Contato Assistencial pode acontecer.",
      "mustSupport" : true
    },
    {
      "id" : "Location.identifier",
      "path" : "Location.identifier",
      "max" : "0"
    },
    {
      "id" : "Location.status",
      "path" : "Location.status",
      "min" : 1,
      "fixedCode" : "active",
      "mustSupport" : true
    },
    {
      "id" : "Location.operationalStatus",
      "path" : "Location.operationalStatus",
      "max" : "0"
    },
    {
      "id" : "Location.name",
      "path" : "Location.name",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Location.alias",
      "path" : "Location.alias",
      "max" : "0"
    },
    {
      "id" : "Location.description",
      "path" : "Location.description",
      "max" : "0"
    },
    {
      "id" : "Location.mode",
      "path" : "Location.mode",
      "min" : 1,
      "fixedCode" : "kind",
      "mustSupport" : true
    },
    {
      "id" : "Location.type",
      "path" : "Location.type",
      "max" : "0"
    },
    {
      "id" : "Location.telecom",
      "path" : "Location.telecom",
      "max" : "0"
    },
    {
      "id" : "Location.address",
      "path" : "Location.address",
      "max" : "0"
    },
    {
      "id" : "Location.physicalType",
      "path" : "Location.physicalType",
      "max" : "0"
    },
    {
      "id" : "Location.position",
      "path" : "Location.position",
      "max" : "0"
    },
    {
      "id" : "Location.managingOrganization",
      "path" : "Location.managingOrganization",
      "max" : "0"
    },
    {
      "id" : "Location.partOf",
      "path" : "Location.partOf",
      "max" : "0"
    },
    {
      "id" : "Location.hoursOfOperation",
      "path" : "Location.hoursOfOperation",
      "max" : "0"
    },
    {
      "id" : "Location.availabilityExceptions",
      "path" : "Location.availabilityExceptions",
      "max" : "0"
    },
    {
      "id" : "Location.endpoint",
      "path" : "Location.endpoint",
      "max" : "0"
    }]
  }
}

```
