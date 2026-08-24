# Motivo do Desfecho - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Motivo do Desfecho 

 
Caracteriza o motivo de conclusão total ou parcial do contato assistencial. 

This Code system is referenced in the definition of the following value sets:

* [Motivo do desfecho do Contato assistencial](ValueSet-BRMotivoDesfecho-1.0.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRMotivoDesfecho",
  "meta" : {
    "lastUpdated" : "2020-03-11T18:16:07.800+00:00"
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRMotivoDesfecho",
  "version" : "1.0.0-release",
  "name" : "BRMotivoDesfecho",
  "title" : "Motivo do Desfecho",
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
  "description" : "Caracteriza o motivo de conclusão total ou parcial do contato assistencial.",
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
    "display" : "Alta clínica"
  },
  {
    "code" : "02",
    "display" : "Alta Voluntária"
  },
  {
    "code" : "03",
    "display" : "Encaminhamento"
  },
  {
    "code" : "04",
    "display" : "Evasão"
  },
  {
    "code" : "05",
    "display" : "Ordem Judicial"
  },
  {
    "code" : "06",
    "display" : "Óbito"
  },
  {
    "code" : "07",
    "display" : "Permanência"
  },
  {
    "code" : "08",
    "display" : "Retorno"
  },
  {
    "code" : "09",
    "display" : "Transferência"
  },
  {
    "code" : "99",
    "display" : "Sem registro no modelo de informação de origem"
  }]
}

```
