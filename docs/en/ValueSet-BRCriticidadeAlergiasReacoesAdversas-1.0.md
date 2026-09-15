# Criticidade de Alergias e Reações Adversas - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## ValueSet: Criticidade de Alergias e Reações Adversas 

 
Indica o potencial de danos nos órgãos críticos do sistema ou consequência de ameaça à vida.. 

 **References** 

* [Alergia ou Reação Adversa](StructureDefinition-BRAlergiaReacaoAdversa-1.0.md)

### Logical Definition (CLD)

 

### Expansion

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRCriticidadeAlergiasReacoesAdversas-1.0",
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
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRCriticidadeAlergiasReacoesAdversas-1.0",
  "version" : "1.0.0-release",
  "name" : "BRCriticidadeAlergiasReacoesAdversas",
  "title" : "Criticidade de Alergias e Reações Adversas",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T20:36:30.5275401+00:00",
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
  "description" : "Indica o potencial de danos nos órgãos críticos do sistema ou consequência de ameaça à vida..",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://hl7.org/fhir/allergy-intolerance-criticality",
      "concept" : [{
        "code" : "low",
        "display" : "Low Risk",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Baixa"
        }]
      },
      {
        "code" : "high",
        "display" : "High Risk",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Alta"
        }]
      },
      {
        "code" : "unable-to-assess",
        "display" : "Unable to Assess Risk",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Indeterminada"
        }]
      }]
    }]
  }
}

```
