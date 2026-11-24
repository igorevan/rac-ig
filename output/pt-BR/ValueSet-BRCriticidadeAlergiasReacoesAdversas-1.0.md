# Criticidade de Alergias e Reações Adversas - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Criticidade de Alergias e Reações Adversas 

 **References** 

* [Alergia ou Reação Adversa](StructureDefinition-BRAlergiaReacaoAdversa-1.0.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRCriticidadeAlergiasReacoesAdversas-1.0",
  "language" : "en",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRCriticidadeAlergiasReacoesAdversas-1.0",
  "version" : "1.0.0",
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
