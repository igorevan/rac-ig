# Tipo de Identificador - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Tipo de Identificador 

 
Classifica o tipo de indicador que está sendo utilizado. 

This Code system is referenced in the definition of the following value sets:

* [BRTipoIdentificadorProcedimento](ValueSet-BRTipoIdentificadorProcedimento-1.0.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRTipoIdentificador",
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoIdentificador",
  "version" : "1.0.0-release",
  "name" : "BRTipoIdentificador",
  "title" : "Tipo de Identificador",
  "status" : "active",
  "experimental" : false,
  "date" : "2020-03-11T18:25:38.8137622+00:00",
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
  "description" : "Classifica o tipo de indicador que está sendo utilizado.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "property" : [{
    "code" : "use",
    "description" : "Uso do Tipo do Identificador",
    "type" : "string"
  }],
  "concept" : [{
    "code" : "AUTH",
    "display" : "Código de Autorização",
    "definition" : "Identificador da permissão para a realização de um procedimento.",
    "property" : [{
      "code" : "use",
      "valueString" : "procedure"
    }]
  },
  {
    "code" : "BRACRA",
    "display" : "Número de inscrição no Conselho Regional de Administração (CRA)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRESS",
    "display" : "Número de inscrição no Conselho Regional de Serviço Social (CRESS)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRB",
    "display" : "Número de inscrição no Conselho Regional de Biblioteconomia (CRB)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRC",
    "display" : "Número de inscrição no Conselho Regional de Contabilidade (CRC)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRECI",
    "display" : "Número de inscrição no Conselho Regional de Corretores de Imóveis (CRECI)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACORECON",
    "display" : "Número de inscrição no Conselho Regional de Economia (CORECON)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACREA",
    "display" : "Número de inscrição no Conselho Regional de Engenharia e Agronomia (CREA)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACONFRE",
    "display" : "Número de inscrição no Conselho Regional de Estatística (CONRE)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRF",
    "display" : "Número de inscrição no Conselho Regional de Farmácia (CRF)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACREFITO",
    "display" : "Número de inscrição no Conselho Regional de Fisioterapia e Terapia Ocupacional (CREFITO)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRMV",
    "display" : "Número de inscrição no Conselho Regional de Medicina Veterinária (CRMV)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRN",
    "display" : "Número de inscrição no Conselho Regional de Nutrição (CRN)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACONRERP",
    "display" : "Número de inscrição no Conselho Regional de Reçações Públicas (CONRERP)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRP",
    "display" : "Número de inscrição no Conselho Regional de Psicologia (CRP)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRQ",
    "display" : "Número de inscrição no Conselho Regional de Química (CRQ)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACORE",
    "display" : "Número de inscrição no Conselho Regional de Representantes Comerciais (CORE)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACREF",
    "display" : "Número de inscrição no Conselho Regional de Educação Física (CREF)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACAU",
    "display" : "Número de inscrição no Conselho Regional de Arquitetura e Urbanismo (CAU)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRBIO",
    "display" : "Número de inscrição no Conselho Regional de Biologia (CRBio)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRBM",
    "display" : "Número da inscrição no Conselho Regional de Biomedicina (CRBM)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRFA",
    "display" : "Número da inscrição no Conselho Regional de Fonoaudiologia (CRFa/CREFONO)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRTR",
    "display" : "Número da inscrição no Conselho Regional de Técnicos em Radiologia (CRTR)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACRT",
    "display" : "Número da inscrição no Conselho Regional dos Técnicos Industriais (CRT)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRAOAB",
    "display" : "Número de inscrição na Ordem dos Advogados do BRAasil (OAB)",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRAIDMIL",
    "display" : "Número da Identidade Militar",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRAIDFUNC",
    "display" : "Número da Identidade Funcional",
    "property" : [{
      "code" : "use",
      "valueString" : "patient"
    }]
  },
  {
    "code" : "BRACNPJ",
    "display" : "Número de inscrição no Cadastro Nacional da Pessoa Jurídica (CNPJ)",
    "property" : [{
      "code" : "use",
      "valueString" : "organization"
    }]
  }]
}

```
