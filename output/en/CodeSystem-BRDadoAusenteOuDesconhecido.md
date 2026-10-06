# Classificação de dados ausentes ou desconhecidos - IPS - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Classificação de dados ausentes ou desconhecidos - IPS 

This Code system is referenced in the definition of the following value sets:

* [Indicativo de prescrição não estruturada ou medicamento não identificado](ValueSet-BRPrescricaoNaoEstruturada.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRDadoAusenteOuDesconhecido",
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRDadoAusenteOuDesconhecido",
  "version" : "1.0.0-release",
  "name" : "BRDadoAusenteOuDesconhecido",
  "title" : "Classificação de dados ausentes ou desconhecidos - IPS",
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
  "description" : "Classificação de dados conhecidos mas ausentes e de dados desconhecidos a partir do International Patient Summary - IPS.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "hierarchyMeaning" : "part-of",
  "content" : "complete",
  "concept" : [{
    "code" : "no-allergy-info",
    "display" : "No information about allergies",
    "definition" : "There is no information available regarding the subject's allergy conditions.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Nenhuma informação sobre alergias"
    }]
  },
  {
    "code" : "no-known-allergies",
    "display" : "No known allergies",
    "definition" : "The subject has no known allergy conditions.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Nenhuma alergia conhecida."
    }],
    "concept" : [{
      "code" : "no-known-medication-allergies",
      "display" : "No known medication allergies",
      "definition" : "The subject has no known medication allergy conditions.",
      "designation" : [{
        "language" : "pt-BR",
        "value" : "Nenhum medicamento para alergia conhecido."
      }]
    },
    {
      "code" : "no-known-environmental-allergies",
      "display" : "No known environmental allergies",
      "definition" : "The subject has no known environmental allergy conditions.",
      "designation" : [{
        "language" : "pt-BR",
        "value" : "Nenhum fator ambiental conhecido para uma dada alergia."
      }]
    },
    {
      "code" : "no-known-food-allergies",
      "display" : "No known food allergies",
      "definition" : "The subject has no known food allergy conditions.",
      "designation" : [{
        "language" : "pt-BR",
        "value" : "Nenhuma alergia alimentar conhecida."
      }]
    }]
  },
  {
    "code" : "no-device-info",
    "display" : "No information about devices",
    "definition" : "There is no information available regarding implanted or external devices for the subject.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Nenhuma informação sobre algum dispositivo."
    }]
  },
  {
    "code" : "no-known-devices",
    "display" : "No known devices in use",
    "definition" : "There are no devices known to be implanted in or used by the subject that have to be reported in this record. This can mean either that there are none known, or that those known are not relevant for the purpose of this record.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Nenhum dispositivo em uso"
    }]
  },
  {
    "code" : "no-immunization-info",
    "display" : "No information about immunizations",
    "definition" : "The subject's history of previous immunizations is not known.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Nenhuma informação sobre imunização"
    }]
  },
  {
    "code" : "no-known-immunizations",
    "display" : "No known immunizations",
    "definition" : "There is no history of previous immunizations for the subject that have to be reported in this record. This can mean either that there are none known, or that those known are not relevant for the purpose of this record.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Nenhuma informação sobre imunização."
    }]
  },
  {
    "code" : "no-medication-info",
    "display" : "No information about medications",
    "definition" : "There is no information available about the subject's medication use or administration.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Sem informação de medicamentos."
    }]
  },
  {
    "code" : "no-known-medications",
    "display" : "No known medications",
    "definition" : "There are no medications for the subject that have to be reported in this record. This can mean either that there are none known, or that those known are not relevant for the purpose of this record.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Sem medicação."
    }]
  },
  {
    "code" : "no-problem-info",
    "display" : "No information about problems",
    "definition" : "There is no information available about the subject's health problems or disabilities.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Nenhuma informação sobre o problema."
    }]
  },
  {
    "code" : "no-known-problems",
    "display" : "No known problems",
    "definition" : "The subject is not known to have any health problems or disabilities that have to be reported in this record. This can mean either that there are none known, or that those known are not relevant for the purpose of this record.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Nenhum problema conhecido."
    }]
  },
  {
    "code" : "no-procedure-info",
    "display" : "No information about past history of procedures",
    "definition" : "There is no information available about the subject's past history of procedures.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Nenhuma informação sobre procedimento."
    }]
  },
  {
    "code" : "no-known-procedures",
    "display" : "No known procedures",
    "definition" : "The subject has no history of procedures that have to be reported in this record. This can mean either that there are none known, or that those known are not relevant for the purpose of this record.",
    "designation" : [{
      "language" : "pt-BR",
      "value" : "Nenhum procedimento conhecido."
    }]
  }]
}

```
