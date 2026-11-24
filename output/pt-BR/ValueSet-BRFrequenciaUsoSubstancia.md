# Frequência de Uso da Substância - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Frequência de Uso da Substância 

 **References** 

* [Medida Observada](StructureDefinition-BRMedidaObservada.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRFrequenciaUsoSubstancia",
  "language" : "en",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRFrequenciaUsoSubstancia",
  "version" : "1.0.0",
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
