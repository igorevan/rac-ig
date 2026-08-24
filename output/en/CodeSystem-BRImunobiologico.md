# Imunobiológico - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## CodeSystem: Imunobiológico 

 
Classifica os tipos de imunobiológicos. 

This Code system is referenced in the definition of the following value sets:

* [Alérgenos](ValueSet-BRAlergenos-1.0.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "BRImunobiologico",
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
  "url" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRImunobiologico",
  "version" : "1.0.0-release",
  "name" : "BRImunobiologico",
  "title" : "Imunobiológico (CodeSystem)",
  "status" : "active",
  "experimental" : false,
  "date" : "2023-01-12T18:40:15.6103207+00:00",
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
  "description" : "Classifica os tipos de imunobiológicos.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "BR"
    }]
  }],
  "caseSensitive" : true,
  "content" : "complete",
  "property" : [{
    "code" : "Name",
    "description" : "Nome técnico completo e oficial do produto, conforme registro junto aos órgãos competentes.",
    "type" : "string"
  },
  {
    "code" : "Category",
    "description" : "Classificação ampla do produto, limitada às categorias: Anticorpo Monoclonal, Diluente, Imunoglobulina, Soro e Vacina.",
    "type" : "string"
  },
  {
    "code" : "inactive",
    "uri" : "http://hl7.org/fhir/concept-properties#inactive",
    "description" : "Status do imunobiológico em que determina se ele está apto para uso no registro de doses aplicadas. Serão aceitos códigos inativos apenas em caso de Transcrição de Caderneta.",
    "type" : "boolean"
  }],
  "concept" : [{
    "code" : "1",
    "display" : "IGHAT",
    "definition" : "imunoglobulina humana antitétano",
    "property" : [{
      "code" : "Name",
      "valueString" : "Imunoglobulina humana antitétano"
    },
    {
      "code" : "Category",
      "valueString" : "Imunoglobulina"
    }]
  },
  {
    "code" : "2",
    "display" : "SAT",
    "definition" : "soro antitetânico",
    "property" : [{
      "code" : "Name",
      "valueString" : "Soro antitetânico"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "3",
    "display" : "SAAR",
    "definition" : "soro antiaracnídico (Loxosceles, Phoneutria, Tityus)",
    "property" : [{
      "code" : "Name",
      "valueString" : "Soro antiaracnídico (Loxosceles, Phoneutria, Tityus)"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "4",
    "display" : "SAESC",
    "definition" : "soro antiescorpiônico",
    "property" : [{
      "code" : "Name",
      "valueString" : "Soro antiescorpiônico"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "5",
    "display" : "DT",
    "definition" : "vacina difteria e tétano infantil",
    "property" : [{
      "code" : "Name",
      "valueString" : "Vacina adsorvida difteria e tétano infantil"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "6",
    "display" : "SAELA",
    "definition" : "soro antielapídico",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro antielapídico (bivalente)"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "7",
    "display" : "SAR",
    "definition" : "soro antirrábico",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro antirrábico"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "8",
    "display" : "SABR",
    "definition" : "soro antibotrópico",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro antibotrópico (pentavalente)"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "9",
    "display" : "HB",
    "definition" : "vacina hepatite B",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina hepatite B (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "10",
    "display" : "SAD",
    "definition" : "soro antidiftérico",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro antidiftérico"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "11",
    "display" : "SABC",
    "definition" : "soro antibotrópico e anticrotálico",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro antibotrópico (pentavalente) e anticrotálico"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "12",
    "display" : "SABL",
    "definition" : "soro antibotrópico e antilaquético",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro antibotrópico (pentavalente) e antilaquético"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "13",
    "display" : "MenAC",
    "definition" : "vacina meningo AC",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina meningocócica AC (polissacarídica)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "14",
    "display" : "VFA",
    "definition" : "vacina febre amarela",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina febre amarela (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "15",
    "display" : "BCG",
    "definition" : "vacina BCG",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina BCG"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "16",
    "display" : "SAC",
    "definition" : "soro anticrotálico",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro anticrotálico"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "17",
    "display" : "Hib",
    "definition" : "vacina Hib",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina Haemophilus influenza B (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "18",
    "display" : "VR embrião de galinha",
    "definition" : "vacina raiva embrião de galinha",
    "property" : [{
      "code" : "inactive",
      "valueBoolean" : true
    },
    {
      "code" : "Name",
      "valueString" : "vacina raiva (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "19",
    "display" : "IGHAVZ",
    "definition" : "imunoglobulina humana antivaricela",
    "property" : [{
      "code" : "Name",
      "valueString" : "imunoglobulina humana antivaricela"
    },
    {
      "code" : "Category",
      "valueString" : "Imunoglobulina"
    }]
  },
  {
    "code" : "20",
    "display" : "IGHAHB",
    "definition" : "imunoglobulina humana anti-hepatite B",
    "property" : [{
      "code" : "Name",
      "valueString" : "imunoglobulina humana anti-hepatite B"
    },
    {
      "code" : "Category",
      "valueString" : "Imunoglobulina"
    }]
  },
  {
    "code" : "21",
    "display" : "VPP23",
    "definition" : "vacina pneumo 23",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina pneumocócica 23-valente (polissacarídica)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "22",
    "display" : "VIP",
    "definition" : "vacina inativada poliomielite",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina poliomelite 1, 2 e 3 (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "23",
    "display" : "IGHAR",
    "definition" : "imunoglobulina humana antirrábica",
    "property" : [{
      "code" : "Name",
      "valueString" : "imunoglobulina humana antirrábica"
    },
    {
      "code" : "Category",
      "valueString" : "Imunoglobulina"
    }]
  },
  {
    "code" : "24",
    "display" : "SCR",
    "definition" : "vacina tríplice viral",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina sarampo, caxumba, rubéola (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "25",
    "display" : "dT",
    "definition" : "vacina difteria e tétano adulto",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida difteria e tétano adulto"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "26",
    "display" : "VPC10",
    "definition" : "vacina pneumo 10",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina pneumocócica 10-valente (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "27",
    "display" : "SALATRO",
    "definition" : "soro antilatrodéctico",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro antilatrodéctico (Latrodectus curacaviensis)"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "28",
    "display" : "VOPb",
    "definition" : "vacina oral poliomielite bivalente",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina poliomielite 1 e 3 (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "29",
    "display" : "Penta acelular",
    "definition" : "vacina penta acelular (DTPa/VIP/Hib)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida difteria, tétano, pertussis (acelular), poliomielite 1, 2 e 3 (inativada) e Haemophilus influenzae B (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "30",
    "display" : "FTp",
    "definition" : "vacina febre tifóide",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina febre tifóide (polissacarídica)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "31",
    "display" : "SALOX",
    "definition" : "soro antiloxoscélico",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro antiloxoscélico (trivalente)"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "32",
    "display" : "SALON",
    "definition" : "soro antilonômico",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro antilonômico"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "33",
    "display" : "INF3",
    "definition" : "vacina influenza trivalente",
    "designation" : [{
      "language" : "en",
      "value" : "Influenza vaccine trivalent"
    },
    {
      "language" : "es",
      "value" : "Vacuna influenza trivalente"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina influenza trivalente (fragmentada, inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "34",
    "display" : "VZ",
    "definition" : "vacina varicela",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina varicela (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "35",
    "display" : "HA virossomal",
    "definition" : "vacina hepatite A (virossomal)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida hepatite A (virossomal)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "36",
    "display" : "SR",
    "definition" : "vacina dupla viral",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina sarampo, rubéola (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "37",
    "display" : "VR",
    "definition" : "vacina raiva (inativada)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina raiva (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "38",
    "display" : "SBOTULTRI",
    "definition" : "soro antibotulínico (trivalente)",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro antibotulínico (trivalente)"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "39",
    "display" : "Tetra",
    "definition" : "vacina DTP/Hib",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida difteria, tétano, pertussis e Haemophilus influenzae B (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "40",
    "display" : "VPC7",
    "definition" : "vacina pneumo 7",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina pneumocócica 7-valente (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "41",
    "display" : "MenC",
    "definition" : "vacina meningo C",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina meningocócica C (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "42",
    "display" : "Penta",
    "definition" : "vacina penta (DTP/HB/Hib)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida difteria, tétano, pertussis, hepatite B (recombinante) e Haemophilus influenzae B (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "43",
    "display" : "Hexa acelular",
    "definition" : "vacina hexa acelular (DTPa/HB/VIP/Hib)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida difteria, tétano, pertussis (acelular), hepatite B (recombinante), poliomielite 1, 2 e 3 (inativada), Haemophilus influenzae B (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "44",
    "display" : "INFH1N1-2009",
    "definition" : "vacina influenza A (H1N1) (inativada, fragmentada)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina influenza tipo A (H1N1) (inativada, fragmentada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "45",
    "display" : "ROTA",
    "definition" : "vacina rotavírus",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina rotavírus humano G1P[8] (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "46",
    "display" : "DTP",
    "definition" : "vacina DTP",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida difteria, tétano e pertussis"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "47",
    "display" : "DTPa",
    "definition" : "vacina DTPa infantil",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida difteria, tétano e pertussis (acelular)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "48",
    "display" : "DILSCR",
    "definition" : "diluente para vacina tríplice viral",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina sarampo, caxumba, rubéola (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "49",
    "display" : "DILVFA",
    "definition" : "diluente para vacina febre amarela",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina febre amarela (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "50",
    "display" : "DILHib",
    "definition" : "diluente para vacina Hib",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina Haemophilus influenzae B (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "51",
    "display" : "Fta",
    "definition" : "vacina febre tifóide (atenuada)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina febre tifóide (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "52",
    "display" : "DILMenAC",
    "definition" : "diluente para vacina meningo AC",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina meningocócica AC (polissacarídica)"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "53",
    "display" : "DILSR",
    "definition" : "diluente para vacina dupla viral",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina sarampo, rubéola (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "54",
    "display" : "DILVAR",
    "definition" : "diluente para vacina varicela",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina varicela (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "55",
    "display" : "HAinf",
    "definition" : "vacina hepatite A infantil",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida hepatite A (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "56",
    "display" : "SCRV",
    "definition" : "vacina tetraviral",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina sarampo, caxumba, rubéola e varicela (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "57",
    "display" : "dTpa",
    "definition" : "vacina dTpa adulto",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida difteria, tétano e pertussis (acelular)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "58",
    "display" : "DTPa/VIP",
    "definition" : "vacina tetra acelular DTPa/VIP",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida difteria, tétano, pertussis (acelular), poliomielite 1, 2 e 3 (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "59",
    "display" : "VPC13",
    "definition" : "vacina pneumo 13",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina pneumocócica 13-valente (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "60",
    "display" : "HPV2",
    "definition" : "vacina HPV bivalente",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina papilomavírus humano 16 e 18 (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "61",
    "display" : "Tétano",
    "definition" : "vacina tétano",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina tétano (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "62",
    "display" : "HA-HBinf",
    "definition" : "vacina hepatite A e B infantil",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida hepatite A e hepatite B (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "63",
    "display" : "HA-HBad",
    "definition" : "vacina hepatite A e B adulto",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida hepatite A e hepatite B (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "64",
    "display" : "INF3-ID",
    "definition" : "vacina influenza trivalente ID",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina influenza trivalente (fragmentada, inativada) intradérmica"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "65",
    "display" : "ROTA5",
    "definition" : "vacina rotavírus pentavalente",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina rotavírus humano/bovino G1, G2, G3, G4 e P1A[8] (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "66",
    "display" : "MenBC",
    "definition" : "vacina meningo BC",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina meningocócica BC (polissacarídica)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "67",
    "display" : "HPV4",
    "definition" : "vacina HPV quadrivalente",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina papilomavírus humano 6, 11, 16 e 18 (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "68",
    "display" : "HPV2",
    "definition" : "vacina HPV bivalente",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina papilomavírus humano 16 e 18 (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "69",
    "display" : "SAB",
    "definition" : "soro antibotulínico AB (bivalente)",
    "property" : [{
      "code" : "Name",
      "valueString" : "soro antibotulínico AB (bivalente)"
    },
    {
      "code" : "Category",
      "valueString" : "Soro"
    }]
  },
  {
    "code" : "70",
    "display" : "Sarampo",
    "definition" : "vacina sarampo",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina sarampo (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "71",
    "display" : "Rubéola",
    "definition" : "vacina rubéola",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina rubéola (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "72",
    "display" : "INFH1N1-2009",
    "definition" : "vacina influenza A (H1N1) (inativada, fragmentada)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina influenza tipo A (H1N1) (inativada, fragmentada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "73",
    "display" : "SCRV",
    "definition" : "vacina sarampo, caxumba, rubéola e varicela",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina sarampo, caxumba, rubéola e varicela (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "74",
    "display" : "MenACWY",
    "definition" : "vacina meningo ACWY",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina meningocócica ACWY (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "75",
    "display" : "VCO",
    "definition" : "vacina cólera oral",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina cólera (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "76",
    "display" : "VHZ",
    "definition" : "vacina herpes-zóster (atenuada)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina herpes-zóster (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "77",
    "display" : "INF4",
    "definition" : "vacina influenza tetravalente",
    "designation" : [{
      "language" : "en",
      "value" : "Influenza vaccine tetravalent"
    },
    {
      "language" : "es",
      "value" : "Vacuna influenza tetravalente"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina influenza tetravalente (fragmentada, inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "78",
    "display" : "MenB",
    "definition" : "vacina meningo B",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida meningocócica B (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "79",
    "display" : "DILBCG",
    "definition" : "diluente para vacina BCG",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina BCG"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "80",
    "display" : "DILVR",
    "definition" : "diluente para vacina raiva (inativada)",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina raiva (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "81",
    "display" : "DILMenC",
    "definition" : "diluente para vacina meningo C",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina meningocócica C (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "82",
    "display" : "Dengue",
    "definition" : "vacina dengue (recombinante e atenuada)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina dengue 1, 2, 3 e 4 (recombinante e atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "83",
    "display" : "HAad",
    "definition" : "vacina hepatite A adulto",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida hepatite A (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "84",
    "display" : "VFA-F",
    "definition" : "vacina febre amarela fracionada",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina febre amarela (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "85",
    "display" : "COVID-19 ASTRAZENECA/FIOCRUZ - COVISHIELD",
    "definition" : "vacina covid-19-recombinante, AstraZeneca/Fiocruz (Covishield)",
    "designation" : [{
      "language" : "en",
      "value" : "XM9QW8 COVID-19 vaccine, non-replicating viral vector"
    },
    {
      "language" : "es",
      "value" : "XM9QW8 Vacuna COVID-19, vector viral no replicante"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina covid-19 (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "86",
    "display" : "COVID-19 SINOVAC/BUTANTAN - CORONAVAC",
    "definition" : "vacina covid-19-inativada, Sinovac/Butantan (Coronavac)",
    "designation" : [{
      "language" : "en",
      "value" : "XM1NL1 COVID-19 vaccine, inactivated virus"
    },
    {
      "language" : "es",
      "value" : "XM1NL1 Vacuna COVID-19, virus inactivado"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida covid-19 (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "87",
    "display" : "COVID-19 PFIZER - COMIRNATY",
    "definition" : "vacina covid-19-RNAm, Pfizer (Comirnaty)",
    "designation" : [{
      "language" : "en",
      "value" : "XM0GQ8 COVID-19 vaccine, RNA based"
    },
    {
      "language" : "es",
      "value" : "XM0GQ8 Vacuna COVID-19, basada en ARN"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina covid-19"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "88",
    "display" : "COVID-19 JANSSEN - Ad26.COV2.S",
    "definition" : "vacina covid-19-recombinante, Janssen (Ad26.COV2.S)",
    "designation" : [{
      "language" : "en",
      "value" : "XM9QW8 COVID-19 vaccine, non-replicating viral vector"
    },
    {
      "language" : "es",
      "value" : "XM9QW8 Vacuna COVID-19, vector viral no replicante"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina covid-19 (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "89",
    "display" : "COVID-19 ASTRAZENECA - ChAdOx1-S",
    "definition" : "vacina covid-19-recombinante, AstraZeneca/Covax (ChAdOx1-S)",
    "designation" : [{
      "language" : "en",
      "value" : "XM9QW8 COVID-19 vaccine, non-replicating viral vector"
    },
    {
      "language" : "es",
      "value" : "XM9QW8 Vacuna COVID-19, vector viral no replicante"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina covid-19 (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "90",
    "display" : "DILSCRV",
    "definition" : "diluente para vacina tetraviral",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina sarampo, caxumba, rubéola e varicela (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "91",
    "display" : "DILVR embrião de galinha",
    "definition" : "diluente para vacina raiva embrião de galinha",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina raiva (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "92",
    "display" : "VR",
    "definition" : "vacina raiva",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina raiva (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "93",
    "display" : "HPV9",
    "definition" : "vacina HPV nonavalente",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina papilomavírus humano 9-valente (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "94",
    "display" : "NaCl 0,9%",
    "definition" : "cloreto de sódio, solução injetável - 0,9%",
    "property" : [{
      "code" : "Name",
      "valueString" : "cloreto de sódio, solução injetável - 0,9%"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  },
  {
    "code" : "95",
    "display" : "COVID-19 GAMALEYA - SPUTNIK V",
    "definition" : "vacina covid-19-recombinante, Gamaleya (Sputnik V)",
    "designation" : [{
      "language" : "en",
      "value" : "XM9QW8 COVID-19 vaccine, non-replicating viral vector"
    },
    {
      "language" : "es",
      "value" : "XM9QW8 Vacuna COVID-19, vector viral no replicante"
    }],
    "property" : [{
      "code" : "inactive",
      "valueBoolean" : true
    },
    {
      "code" : "Name",
      "valueString" : "vacina covid-19 (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "96",
    "display" : "COVID-19 BHARAT - COVAXIN",
    "definition" : "vacina covid-19-inativada, Bharat (Covaxin)",
    "designation" : [{
      "language" : "en",
      "value" : "XM1NL1 COVID-19 vaccine, inactivated virus"
    },
    {
      "language" : "es",
      "value" : "XM1NL1 Vacuna COVID-19, virus inactivado"
    }],
    "property" : [{
      "code" : "inactive",
      "valueBoolean" : true
    },
    {
      "code" : "Name",
      "valueString" : "vacina adsorvida covid-19 (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "97",
    "display" : "COVID-19 MODERNA - SPIKEVAX",
    "definition" : "vacina covid-19-RNAm, Moderna (Spikevax)",
    "designation" : [{
      "language" : "en",
      "value" : "XM0GQ8 COVID-19 vaccine, RNA based"
    },
    {
      "language" : "es",
      "value" : "XM0GQ8 Vacuna COVID-19, basada en ARN"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina covid-19"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "98",
    "display" : "COVID-19 SINOVAC - CORONAVAC",
    "definition" : "vacina covid-19-inativada, Sinovac (Coronavac)",
    "designation" : [{
      "language" : "en",
      "value" : "XM1NL1 COVID-19 vaccine, inactivated virus"
    },
    {
      "language" : "es",
      "value" : "XM1NL1 Vacuna COVID-19, virus inactivado"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida covid-19 (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "99",
    "display" : "COVID-19 PFIZER - COMIRNATY PEDIÁTRICA",
    "definition" : "vacina covid-19-RNAm, Pfizer (Comirnaty) pediátrica",
    "designation" : [{
      "language" : "en",
      "value" : "XM0GQ8 COVID-19 vaccine, RNA based"
    },
    {
      "language" : "es",
      "value" : "XM0GQ8 Vacuna COVID-19, basada en ARN"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina covid-19"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "100",
    "display" : "VVS",
    "definition" : "vacina varíola símia (atenuada)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina varíola símia (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "101",
    "display" : "VHZR",
    "definition" : "vacina herpes-zóster (recombinante)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina herpes-zóster (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "102",
    "display" : "COVID-19 PFIZER - COMIRNATY PEDIÁTRICA MENOR DE 5 ANOS",
    "definition" : "vacina covid-19-RNAm, Pfizer (Comirnaty) pediátrica menor de 5 anos",
    "designation" : [{
      "language" : "en",
      "value" : "XM0GQ8 COVID-19 vaccine, RNA based"
    },
    {
      "language" : "es",
      "value" : "XM0GQ8 Vacuna COVID-19, basada en ARN"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina covid-19"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "103",
    "display" : "COVID-19 PFIZER - COMIRNATY BIVALENTE",
    "definition" : "vacina covid-19-RNAm, Pfizer (Comirnaty) bivalente",
    "designation" : [{
      "language" : "en",
      "value" : "XM0GQ8 COVID-19 vaccine, RNA based"
    },
    {
      "language" : "es",
      "value" : "XM0GQ8 Vacuna COVID-19, basada en ARN"
    }],
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina covid-19 bivalente"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "104",
    "display" : "DNG",
    "definition" : "vacina dengue (atenuada)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina dengue 1, 2, 3 e 4 (atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "105",
    "display" : "COVID-19-SPIKEVAX BI",
    "definition" : "vacina covid-19-RNAm, Moderna (Spikevax) bivalente",
    "property" : [{
      "code" : "inactive",
      "valueBoolean" : true
    },
    {
      "code" : "Name",
      "valueString" : "Vacina covid-19 bivalente (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "106",
    "display" : "VPC15",
    "definition" : "vacina pneumo 15",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida pneumocócica 15-valente (conjugada, polissacarídica)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "107",
    "display" : "VPC20",
    "definition" : "vacina pneumo 20",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina pneumocócica 20-valente (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "108",
    "display" : "VVSR-Rec",
    "definition" : "vacina vírus sincicial respiratório A e B (recombinante)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina vírus sincicial respiratório A e B (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "109",
    "display" : "VVSR-RecAdj",
    "definition" : "vacina vírus sincicial respiratório (recombinante, adjuvada)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina vírus sincicial respiratório (recombinante, adjuvada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "110",
    "display" : "INF4-alta dosagem",
    "definition" : "vacina influenza tetravalente - alta dosagem",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina influenza tetravalente (fragmentada, inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "111",
    "display" : "dTpa/VIP",
    "definition" : "vacina tetra acelular dTpa/VIP",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina adsorvida difteria, tétano, pertussis (acelular), poliomielite 1, 2 e 3 (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "112",
    "display" : "COVID-19 SERUM/ZALIKA",
    "definition" : "vacina covid-19-recombinante, Serum/Zalika",
    "property" : [{
      "code" : "Name",
      "valueString" : "Vacina covid-19 (recombinante)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "113",
    "display" : "CHIKUNGUNYA",
    "definition" : "vacina chikungunya (recombinante e atenuada)",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina chikungunya (recombinante e atenuada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "114",
    "display" : "COVID-19 SINOPHARM",
    "definition" : "vacina covid-19-inativada, Sinopharm",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina covid-19 (inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "115",
    "display" : "NIRSEVIMABE 0,5ml",
    "definition" : "nirsevimabe 0,5ml",
    "property" : [{
      "code" : "Name",
      "valueString" : "nirsevimabe 0,5ml"
    },
    {
      "code" : "Category",
      "valueString" : "Anticorpo Monoclonal"
    }]
  },
  {
    "code" : "116",
    "display" : "NIRSEVIMABE 1,0ml",
    "definition" : "nirsevimabe 1,0ml",
    "property" : [{
      "code" : "Name",
      "valueString" : "nirsevimabe 1,0ml"
    },
    {
      "code" : "Category",
      "valueString" : "Anticorpo Monoclonal"
    }]
  },
  {
    "code" : "117",
    "display" : "INF3-alta dosagem",
    "definition" : "vacina influenza trivalente - alta dosagem",
    "property" : [{
      "code" : "Name",
      "valueString" : "vacina influenza trivalente (fragmentada, inativada)"
    },
    {
      "code" : "Category",
      "valueString" : "Vacina"
    }]
  },
  {
    "code" : "118",
    "display" : "DILMenACWY",
    "definition" : "diluente para vacina meningo ACWY",
    "property" : [{
      "code" : "Name",
      "valueString" : "diluente para vacina meningocócica ACWY (conjugada)"
    },
    {
      "code" : "Category",
      "valueString" : "Diluente"
    }]
  }]
}

```
