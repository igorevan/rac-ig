# Tipo de Observação (ValueSet) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## ValueSet: Tipo de Observação 

 
Tipo de Observação. 

 **References** 

* [Medida Observada](StructureDefinition-BRMedidaObservada.md)
* [Observação Descritiva](StructureDefinition-BRObservacaoDescritiva-1.0.md)

### Logical Definition (CLD)

 

### Expansion

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRTipoObservacao-1.0",
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
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTipoObservacao-1.0",
  "version" : "1.0.0-release",
  "name" : "BRTipoObservacao",
  "title" : "Tipo de Observação",
  "status" : "active",
  "experimental" : false,
  "date" : "2022-05-23T10:37:59.848+00:00",
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
  "immutable" : false,
  "copyright" : "This material contains content from LOINC (http://loinc.org). LOINC is copyright © 1995-2020, Regenstrief Institute, Inc. and the Logical Observation Identifiers Names and Codes (LOINC) Committee and is available at no cost under the license at http://loinc.org/license. LOINC® is a registered United States trademark of Regenstrief Institute, Inc",
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoObservacao"
    },
    {
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTabelaSUS",
      "concept" : [{
        "code" : "0301100039"
      }]
    },
    {
      "system" : "http://loinc.org",
      "concept" : [{
        "code" : "8665-2",
        "display" : "Last menstrual period start date",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Data da Última Menstruação"
        }]
      },
      {
        "code" : "56832-9",
        "display" : "Type of substance abused",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Exposição à Substâncias"
        }]
      },
      {
        "code" : "11996-6",
        "display" : "Pregnancies",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Quantidade de Gestações"
        }]
      },
      {
        "code" : "63895-7",
        "display" : "Breastfeeding status",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Tipo de Aleitamento Materno"
        }]
      },
      {
        "code" : "29463-7",
        "display" : "Body weight",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Peso Corporal"
        }]
      },
      {
        "code" : "8480-6",
        "display" : "Systolic blood pressure",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Pressão Arterial Sistólica"
        }]
      },
      {
        "code" : "8462-4",
        "display" : "Diastolic blood pressure",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Pressão Arterial Diastólica"
        }]
      },
      {
        "code" : "8280-0",
        "display" : "Waist Circumference at umbilicus by Tape measure",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Circuferência Abdominal"
        }]
      },
      {
        "code" : "9843-4",
        "display" : "Head Occipital-frontal circumference",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Perímetro Cefálico"
        }]
      },
      {
        "code" : "8302-2",
        "display" : "Body height",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Altura"
        }]
      },
      {
        "code" : "11885-1",
        "display" : "Gestational age Estimated from last menstrual period",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Idade Gestacional"
        }]
      },
      {
        "code" : "11612-9",
        "display" : "Abortions",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Quantidade de Abortos"
        }]
      },
      {
        "code" : "48767-8",
        "display" : "Annotation comment [Interpretation] Narrative",
        "designation" : [{
          "language" : "pt-BR",
          "value" : "Anotação de Comentário para Narrativa [Interpretação]"
        }]
      }]
    }]
  }
}

```
