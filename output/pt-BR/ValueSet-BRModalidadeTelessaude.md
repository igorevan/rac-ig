# Modalidade de Telessaúde (ValueSet) - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0

## ValueSet: Modalidade de Telessaúde (ValueSet) 

 **References** 

* [Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md)

### Definição lógica (CLD)

 

### Expansão

-------

 [Descrição do(s) quadro(s) acima](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "BRModalidadeTelessaude",
  "language" : "pt-BR",
  "url" : "http://www.saude.gov.br/fhir/r4/ValueSet/BRModalidadeTelessaude",
  "version" : "1.0.0",
  "name" : "BRModalidadeTelessaude",
  "title" : "Modalidade de Telessaúde (ValueSet)",
  "status" : "active",
  "experimental" : false,
  "date" : "2026-06-24T12:05:18.2868027+00:00",
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
  "description" : "Conjunto de códigos utilizados para identificar as modalidades de telessaúde no contexto do atendimento clínico.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "compose" : {
    "include" : [{
      "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRModalidadeTelessaude"
    }]
  }
}

```
