# Posição do Indivíduo (ValueSet) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Posição do Indivíduo 

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
  "id" : "BRPosicaoIndividuo",
  "language" : "en",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRPosicaoIndividuo",
  "version" : "1.0.0",
  "name" : "BRPosicaoIndividuo",
  "title" : "Posição do Indivíduo",
  "status" : "active",
  "experimental" : false,
  "date" : "2022-05-23T11:15:35.881+00:00",
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
  "description" : "ValueSet utilizado para identificar a posição do indivíduo no momento da ação / procedimento.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "immutable" : false,
  "copyright" : "This material contains content from LOINC (http://loinc.org). LOINC is copyright © 1995-2020, Regenstrief Institute, Inc. and the Logical Observation Identifiers Names and Codes (LOINC) Committee and is available at no cost under the license at http://loinc.org/license. LOINC® is a registered United States trademark of Regenstrief Institute, Inc",
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRPosicaoIndividuo"
    },
    {
      "system" : "http://loinc.org",
      "concept" : [{
        "code" : "LA11868-9",
        "display" : "Sitting",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Sentado"
        }]
      },
      {
        "code" : "LA11869-7",
        "display" : "Lying",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Deitado"
        }]
      },
      {
        "code" : "LA11870-5",
        "display" : "Standing",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "De pé"
        }]
      }]
    }]
  }
}

```
