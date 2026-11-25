# Turno - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## Extensão: Turno 

**Context of Use**

**Usage info**

**Usos:**

* Usa este Extensão: [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md)
* Exemplos para este Extensão: [Bundle/bundle-example-rac-1](Bundle-bundle-example-rac-1.md), [Bundle/bundle-example-rac-2](Bundle-bundle-example-rac-2.md) and [Bundle/bundle-example-rac-tc](Bundle-bundle-example-rac-tc.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/br.gov.saude.rac.fhir|current/StructureDefinition/StructureDefinition-BRTurno.json)

### Visões formais do conteúdo da extensão

 [Descrição de perfis, diferenciais, instantâneos e suas representações](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

*  [Tabela diferencial](#tabs-diff) 
*  [Tabela de instantâneos](#tabs-snap) 
*  [Estatísticas/Referências](#tabs-summ) 
*  [Todas](#tabs-all) 

Esta estrutura deriva de [Extension](http://hl7.org/fhir/R4/extensibility.html#Extension) 

#### Terminologia Ligações (Diferencial)

#### Terminologia Ligações

#### Restrições

Esta estrutura deriva de [Extension](http://hl7.org/fhir/R4/extensibility.html#Extension) 

 **Visão Diferencial** 

Esta estrutura deriva de [Extension](http://hl7.org/fhir/R4/extensibility.html#Extension) 

#### Terminologia Ligações (Diferencial)

 **Visão Completa** 

#### Terminologia Ligações

#### Restrições

Esta estrutura deriva de [Extension](http://hl7.org/fhir/R4/extensibility.html#Extension) 

 

Outras representações do perfil: [CSV](../StructureDefinition-BRTurno.csv), [Excel](../StructureDefinition-BRTurno.xlsx), [Schematron](../StructureDefinition-BRTurno.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "BRTurno",
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRTurno",
  "version" : "1.0.0",
  "name" : "BRTurno",
  "title" : "Turno",
  "status" : "active",
  "experimental" : false,
  "date" : "2026-11-25T10:11:02-03:00",
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
  "description" : "Extensão para descrever uma unidade de tempo referenciada pelo UCUM.",
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
  }],
  "kind" : "complex-type",
  "abstract" : false,
  "context" : [{
    "type" : "element",
    "expression" : "MedicationRequest"
  }],
  "type" : "Extension",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Extension",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Extension.id",
      "path" : "Extension.id",
      "max" : "0"
    },
    {
      "id" : "Extension.url",
      "path" : "Extension.url",
      "fixedUri" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRTurno"
    },
    {
      "id" : "Extension.value[x]",
      "path" : "Extension.value[x]",
      "short" : "Turno do dia",
      "definition" : "Em qual momento do dia ocorre o consumo do medicamento: Manhã, tarde, noite.",
      "type" : [{
        "code" : "code"
      }],
      "binding" : {
        "strength" : "required",
        "description" : "Define o turno do dia",
        "valueSet" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRTurno"
      }
    }]
  }
}

```
