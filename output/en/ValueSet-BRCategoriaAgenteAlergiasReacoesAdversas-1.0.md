# Categoria do Agente da Alergia ou Reação Adversa - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## ValueSet: Categoria do Agente da Alergia ou Reação Adversa 

 
Categoriza a substância responsável por causar uma alergia ou reação adversa. 

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
  "id" : "BRCategoriaAgenteAlergiasReacoesAdversas-1.0",
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
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRCategoriaAgenteAlergiasReacoesAdversas-1.0",
  "version" : "1.0.0-release",
  "name" : "BRCategoriaAgenteAlergiasReacoesAdversas",
  "title" : "Categoria do Agente da Alergia ou Reação Adversa",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-09-20T20:37:36.0254538+00:00",
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
  "description" : "Categoriza a substância responsável por causar uma alergia ou reação adversa.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "compose" : {
    "include" : [{
      "system" : "http://hl7.org/fhir/allergy-intolerance-category",
      "concept" : [{
        "code" : "food",
        "display" : "Food",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Alimento - Substância recebida pelo corpo que proporciona nutrição. (DeCS/BVS)"
        }]
      },
      {
        "code" : "medication",
        "display" : "Medication",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Medicamento - Substâncias farmacêuticas complexas, preparações ou produtos de origem orgânica geralmente obtidos por métodos ou ensaios biológicos. (DeCS/BVS) Ex.: vacinas, soros, hormônios, antitoxinas etc."
        }]
      },
      {
        "code" : "biologic",
        "display" : "Biologic",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Biológica - Drogas dirigidas para uso humano ou veterinário, apresentadas em sua formulação final. Estão incluídos aqui os materiais usados na preparação e/ou na formulação final. (DeCS/BVS)"
        }]
      },
      {
        "code" : "environment",
        "display" : "Environment",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Fator Externo/Ambiental - Quaisquer substâncias encontradas no meio ambiente, incluindo qualquer substância ainda não classificada como alimento, medicamento ou biológico (Tradução livre da definição original do HL7)."
        }]
      }]
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-NullFlavor",
      "concept" : [{
        "code" : "OTH",
        "display" : "other",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Outras Substâncias - Qualquer outra substância encontrada no ambiente e que não pode ser classificada como alimento, medicamento ou biológica (Tradução livre da definição original do HL7)."
        }]
      }]
    }]
  }
}

```
