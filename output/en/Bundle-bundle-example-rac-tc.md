# Bundle de Exemplo do Registro de Atendimento Clínico (RAC) - Modalidade de Teleconsulta - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## Example Bundle: Bundle de Exemplo do Registro de Atendimento Clínico (RAC) - Modalidade de Teleconsulta



## Resource Content

```json
{
  "resourceType" : "Bundle",
  "id" : "bundle-example-rac-tc",
  "meta" : {
    "lastUpdated" : "2022-05-09T18:11:18.946402Z"
  },
  "identifier" : {
    "system" : "http://www.saude.gov.br/fhir/r4/NamingSystem/BRRNDS-1",
    "value" : "4629213170263-312915-F461111112-IF46111112M312915.EUT-82313"
  },
  "type" : "document",
  "timestamp" : "2022-05-09T18:11:19.005486Z",
  "entry" : [{
    "fullUrl" : "urn:uuid:transient-0",
    "resource" : {
      "resourceType" : "Composition",
      "id" : "transient-0",
      "meta" : {
        "lastUpdated" : "2022-05-09T17:28:34.132629Z",
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRRegistroAtendimentoClinico"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Composition_transient-0\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Composition transient-0</b></p><a name=\"transient-0\"> </a><a name=\"hctransient-0\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\">Última atualização: 2022-05-09 17:28:34+0000</p><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRRegistroAtendimentoClinico.html\">Registro de Atendimento Clínico</a></p></div><p><b>status</b>: Final</p><p><b>type</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoDocumento RAC}\">Registro de Atendimento Clínico</span></p><p><b>category</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRModalidadeAssistencial 04}\">Atenção Hospitalar</span></p><p><b>date</b>: 2022-05-09</p><p><b>author</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BREstabelecimentoSaude-1.0</code>/3191384</p><p><b>title</b>: Registro de Atendimento Clínico</p></div>"
      },
      "status" : "final",
      "type" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoDocumento",
          "code" : "RAC"
        }]
      },
      "category" : [{
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRModalidadeAssistencial",
          "code" : "04"
        }]
      }],
      "subject" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value" : "819217217061851"
        }
      },
      "date" : "2022-05-09",
      "author" : [{
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BREstabelecimentoSaude-1.0",
          "value" : "3191384"
        }
      }],
      "title" : "Registro de Atendimento Clínico",
      "section" : [{
        "entry" : [{
          "reference" : "urn:uuid:transient-1"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-2"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-3"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-6"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-7"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-8"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-9"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-10"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-11"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-12"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-13"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-14"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-15"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-16"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-17"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-18"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-21"
        }]
      },
      {
        "entry" : [{
          "reference" : "urn:uuid:transient-22"
        }]
      }]
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-1",
    "resource" : {
      "resourceType" : "Encounter",
      "id" : "transient-1",
      "meta" : {
        "lastUpdated" : "2022-05-09T17:31:16.551205Z",
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRContatoAssistencial-1.0"]
      },
      "text" : {
        "status" : "extensions",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Encounter_transient-1\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Encounter transient-1</b></p><a name=\"transient-1\"> </a><a name=\"hctransient-1\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\">Última atualização: 2022-05-09 17:31:16+0000</p><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRContatoAssistencial-1.0.html\">Contato Assistencial</a></p></div><p><b>status</b>: Finished</p><p><b>class</b>: <a href=\"CodeSystem-BRModalidadeAssistencial.html#BRModalidadeAssistencial-04\">Modalidade Assistencial: 04</a> (Atenção Hospitalar)</p><p><b>type</b>: <span title=\"Códigos:{http://saude.gov.br/fhir/CodeSystem/BRModalidadeTelessaude teleconsulta}\">teleconsulta</span></p><p><b>priority</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRCaraterAtendimento 01}\">Eletivo</span></p><p><b>subject</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0</code>/819217217061851</p><blockquote><p><b>participant</b></p><p><b>Ocupação</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRCBO 223505}\">ENFERMEIRO</span></p><p><b>Identificador Nacional de Equipe</b>: 2</p><p><b>type</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRResponsabilidadeParticipante solicitante}\">Profissional que solicitou o Contato Assistencial</span></p><p><b>individual</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRLotacaoProfissional-1.0</code>/815113499149874-3191384</p></blockquote><p><b>period</b>: 2022-04-09 --&gt; 2022-05-09</p><p><b>reasonReference</b>: <a href=\"Bundle-bundle-example-rac-tc.html#urn-uuid-transient-4\">Observation 48767-8</a></p><blockquote><p><b>diagnosis</b></p><p><b>condition</b>: <a href=\"Bundle-bundle-example-rac-tc.html#urn-uuid-transient-2\">Condition Varizes esofagianas sem sangramento</a></p><p><b>use</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRPapelProblemaDiagnostico NAD}\">Diagnosis not present on admission</span></p><p><b>rank</b>: 1</p></blockquote><blockquote><p><b>diagnosis</b></p><p><b>condition</b>: <a href=\"Bundle-bundle-example-rac-tc.html#urn-uuid-transient-3\">Procedure CONSULTA DE PROFISSIONAIS DE NIVEL SUPERIOR NA ATENÇÃO ESPECIALIZADA (EXCETO MÉDICO)</a></p></blockquote><h3>Hospitalizations</h3><table class=\"grid\"><tr><td style=\"display: none\">-</td><td><b>Extension</b></td><td><b>AdmitSource</b></td><td><b>DischargeDisposition</b></td></tr><tr><td style=\"display: none\">*</td><td/><td><span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRProcedencia 99}\">Informação ausente no modelo de origem</span></td><td><span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRMotivoDesfecho 06}\">Óbito</span></td></tr></table><h3>Locations</h3><table class=\"grid\"><tr><td style=\"display: none\">-</td><td><b>Location</b></td></tr><tr><td style=\"display: none\">*</td><td><a href=\"Bundle-bundle-example-rac-tc.html#urn-uuid-transient-5\">Estabelecimento de saúde</a></td></tr></table><p><b>serviceProvider</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BREstabelecimentoSaude-1.0</code>/162338254590005</p></div>"
      },
      "status" : "finished",
      "class" : {
        "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRModalidadeAssistencial",
        "code" : "04"
      },
      "type" : [{
        "coding" : [{
          "system" : "http://saude.gov.br/fhir/CodeSystem/BRModalidadeTelessaude",
          "code" : "teleconsulta"
        }]
      }],
      "priority" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRCaraterAtendimento",
          "code" : "01"
        }]
      },
      "subject" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value" : "819217217061851"
        }
      },
      "participant" : [{
        "extension" : [{
          "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BROcupacao-1.0",
          "valueCodeableConcept" : {
            "coding" : [{
              "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRCBO",
              "code" : "223505"
            }]
          }
        },
        {
          "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIdentificacaoEquipe-1.0",
          "valueInteger" : 2
        }],
        "type" : [{
          "coding" : [{
            "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRResponsabilidadeParticipante",
            "code" : "solicitante"
          }]
        }],
        "individual" : {
          "identifier" : {
            "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRLotacaoProfissional-1.0",
            "value" : "815113499149874-3191384"
          }
        }
      }],
      "period" : {
        "start" : "2022-04-09",
        "end" : "2022-05-09"
      },
      "reasonReference" : [{
        "reference" : "urn:uuid:transient-4"
      }],
      "diagnosis" : [{
        "condition" : {
          "reference" : "urn:uuid:transient-2"
        },
        "use" : {
          "coding" : [{
            "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRPapelProblemaDiagnostico",
            "code" : "NAD"
          }]
        },
        "rank" : 1
      },
      {
        "condition" : {
          "extension" : [{
            "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRFinanciamento-1.0",
            "valueCodeableConcept" : {
              "coding" : [{
                "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRFinanciamento",
                "code" : "01"
              }]
            }
          }],
          "reference" : "urn:uuid:transient-3"
        }
      }],
      "hospitalization" : {
        "extension" : [{
          "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BROutrasInformacoes",
          "valueAnnotation" : {
            "time" : "2022-05-09",
            "text" : "Paciente se queixando da presença de sangue na saliva."
          }
        }],
        "admitSource" : {
          "coding" : [{
            "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRProcedencia",
            "code" : "99"
          }]
        },
        "dischargeDisposition" : {
          "coding" : [{
            "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRMotivoDesfecho",
            "code" : "06"
          }]
        }
      },
      "location" : [{
        "location" : {
          "reference" : "urn:uuid:transient-5"
        }
      }],
      "serviceProvider" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BREstabelecimentoSaude-1.0",
          "value" : "162338254590005"
        }
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-2",
    "resource" : {
      "resourceType" : "Condition",
      "id" : "transient-2",
      "meta" : {
        "lastUpdated" : "2022-05-09T17:37:55.000322Z",
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRProblemaDiagnostico"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Condition_transient-2\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Condition transient-2</b></p><a name=\"transient-2\"> </a><a name=\"hctransient-2\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\">Última atualização: 2022-05-09 17:37:55+0000</p><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRProblemaDiagnostico.html\">Problema / Diagnóstico</a></p></div><p><b>clinicalStatus</b>: <span title=\"Códigos:{http://terminology.hl7.org/CodeSystem/condition-clinical active}\">Active</span></p><p><b>category</b>: <span title=\"Códigos:{http://terminology.hl7.org/CodeSystem/condition-category encounter-diagnosis}\">Encounter Diagnosis</span></p><p><b>code</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRCID10 I859}\">Varizes esofagianas sem sangramento</span></p><p><b>subject</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0</code>/819217217061851</p><p><b>note</b>: </p><blockquote><div><p>Varizes esofagianas sem sangramento.</p>\n</div></blockquote></div>"
      },
      "clinicalStatus" : {
        "coding" : [{
          "system" : "http://terminology.hl7.org/CodeSystem/condition-clinical",
          "code" : "active"
        }]
      },
      "category" : [{
        "coding" : [{
          "system" : "http://terminology.hl7.org/CodeSystem/condition-category",
          "code" : "encounter-diagnosis"
        }]
      }],
      "code" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRCID10",
          "code" : "I859"
        }]
      },
      "subject" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value" : "819217217061851"
        }
      },
      "note" : [{
        "text" : "Varizes esofagianas sem sangramento."
      }]
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-3",
    "resource" : {
      "resourceType" : "Procedure",
      "id" : "transient-3",
      "meta" : {
        "lastUpdated" : "2022-05-09T17:39:08.701859Z",
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRProcedimentoRealizado-1.0"]
      },
      "text" : {
        "status" : "extensions",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Procedure_transient-3\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Procedure transient-3</b></p><a name=\"transient-3\"> </a><a name=\"hctransient-3\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\">Última atualização: 2022-05-09 17:39:08+0000</p><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRProcedimentoRealizado-1.0.html\">Procedimento Realizado</a></p></div><p><b>Quantidade</b>: 23</p><p><b>identifier</b>: Código de Autorização/462921313170263</p><p><b>status</b>: Completed</p><p><b>code</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRTabelaSUS 0301010048}\">CONSULTA DE PROFISSIONAIS DE NIVEL SUPERIOR NA ATENÇÃO ESPECIALIZADA (EXCETO MÉDICO)</span></p><p><b>subject</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0</code>/819217217061851</p><p><b>performed</b>: 2022-05-09</p><h3>Performers</h3><table class=\"grid\"><tr><td style=\"display: none\">-</td><td><b>Extension</b></td><td><b>Function</b></td><td><b>Actor</b></td><td><b>OnBehalfOf</b></td></tr><tr><td style=\"display: none\">*</td><td/><td><span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRCBO 223605}\">FISIOTERAPEUTA GERAL</span></td><td>Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRLotacaoProfissional-1.0</code>/815113499149874-3191384</td><td>Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BREstabelecimentoSaude-1.0</code>/162338254590005</td></tr></table></div>"
      },
      "extension" : [{
        "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRQuantidade-1.0",
        "valuePositiveInt" : 23
      }],
      "identifier" : [{
        "type" : {
          "coding" : [{
            "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoIdentificador",
            "code" : "AUTH"
          }]
        },
        "value" : "462921313170263"
      }],
      "status" : "completed",
      "code" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTabelaSUS",
          "code" : "0301010048"
        }]
      },
      "subject" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value" : "819217217061851"
        }
      },
      "performedDateTime" : "2022-05-09",
      "performer" : [{
        "extension" : [{
          "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIdentificacaoEquipe-1.0",
          "valueInteger" : 2
        }],
        "function" : {
          "coding" : [{
            "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRCBO",
            "code" : "223605"
          }]
        },
        "actor" : {
          "identifier" : {
            "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRLotacaoProfissional-1.0",
            "value" : "815113499149874-3191384"
          }
        },
        "onBehalfOf" : {
          "identifier" : {
            "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BREstabelecimentoSaude-1.0",
            "value" : "162338254590005"
          }
        }
      }]
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-4",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-4",
      "meta" : {
        "lastUpdated" : "2022-05-09T17:37:55.000322Z",
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRObservacaoDescritiva-1.0"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-4\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-4</b></p><a name=\"transient-4\"> </a><a name=\"hctransient-4\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\">Última atualização: 2022-05-09 17:37:55+0000</p><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRObservacaoDescritiva-1.0.html\">Observação Descritiva</a></p></div><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 48767-8}\">48767-8</span></p><p><b>subject</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0</code>/819217217061851</p><p><b>issued</b>: 2022-05-09 17:39:08+0000</p><p><b>value</b>: Varizes esofagianas sem sangramento.</p></div>"
      },
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "48767-8"
        }]
      },
      "subject" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value" : "819217217061851"
        }
      },
      "issued" : "2022-05-09T17:39:08.701859Z",
      "valueString" : "Varizes esofagianas sem sangramento."
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-5",
    "resource" : {
      "resourceType" : "Location",
      "id" : "transient-5",
      "meta" : {
        "lastUpdated" : "2022-05-09T17:37:55.000322Z",
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRLocalAtendimento-1.0"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Location_transient-5\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Location transient-5</b></p><a name=\"transient-5\"> </a><a name=\"hctransient-5\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\">Última atualização: 2022-05-09 17:37:55+0000</p><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRLocalAtendimento-1.0.html\">Local de Atendimento</a></p></div><p style=\"border: 1px #661aff solid; background-color: #e6e6ff; padding: 10px;\">Estabelecimento de saúde</p><hr/><table class=\"grid\"><tr><td style=\"background-color: #f3f5da\" title=\"The status of the location\">Status:</td><td>Active</td><td style=\"background-color: #f3f5da\" title=\"Whether this describes a specific location, or a class of locations\">Mode:</td><td>Kind</td></tr></table></div>"
      },
      "status" : "active",
      "name" : "Estabelecimento de saúde",
      "mode" : "kind"
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-6",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-6",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada"]
      },
      "text" : {
        "status" : "extensions",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-6\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-6</b></p><a name=\"transient-6\"> </a><a name=\"hctransient-6\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedidaObservada.html\">Medida Observada</a></p></div><p><b>Origem da Medição</b>: <span title=\"Códigos:{http://loinc.org 3137-7}\">Body height Measured</span></p><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 29463-7}\">29463-7</span></p><p><b>value</b>: 1.83(unit m from https://www.hl7.org/fhir/valueset-ucum-common.html)<span style=\"background: LightGoldenRodYellow\"> (Detalhes: valueset-ucum-common.html códigom = 'm')</span></p><p><b>method</b>: <span title=\"Códigos:{http://loinc.org LA11870-5}\">Standing</span></p></div>"
      },
      "extension" : [{
        "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BROrigemMedida",
        "valueCodeableConcept" : {
          "coding" : [{
            "system" : "http://loinc.org",
            "code" : "3137-7"
          }]
        }
      }],
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "29463-7"
        }]
      },
      "valueQuantity" : {
        "value" : 1.83,
        "system" : "https://www.hl7.org/fhir/valueset-ucum-common.html",
        "code" : "m"
      },
      "method" : {
        "coding" : [{
          "system" : "http://loinc.org",
          "code" : "LA11870-5"
        }]
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-7",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-7",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-7\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-7</b></p><a name=\"transient-7\"> </a><a name=\"hctransient-7\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedidaObservada.html\">Medida Observada</a></p></div><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 8280-0}\">8280-0</span></p><p><b>value</b>: 135.5(unit cm from https://www.hl7.org/fhir/valueset-ucum-common.html)<span style=\"background: LightGoldenRodYellow\"> (Detalhes: valueset-ucum-common.html códigocm = 'cm')</span></p></div>"
      },
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "8280-0"
        }]
      },
      "valueQuantity" : {
        "value" : 135.5,
        "system" : "https://www.hl7.org/fhir/valueset-ucum-common.html",
        "code" : "cm"
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-8",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-8",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-8\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-8</b></p><a name=\"transient-8\"> </a><a name=\"hctransient-8\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedidaObservada.html\">Medida Observada</a></p></div><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 8665-2}\">8665-2</span></p><p><b>value</b>: 2022-05-23</p></div>"
      },
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "8665-2"
        }]
      },
      "valueDateTime" : "2022-05-23"
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-9",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-9",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-9\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-9</b></p><a name=\"transient-9\"> </a><a name=\"hctransient-9\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedidaObservada.html\">Medida Observada</a></p></div><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 56832-9}\">56832-9</span></p><p><b>effective</b>: Código </p><p><b>value</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoSubstanciaUso alcool}\">Bebidas Alcóolicas</span></p><p><b>note</b>: </p><blockquote><div><p>Uso ocasional de cannabis.</p>\n</div></blockquote></div>"
      },
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "56832-9"
        }]
      },
      "effectiveTiming" : {
        "code" : {
          "coding" : [{
            "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRFrequenciaUsoSubstancia",
            "code" : "uma-ou-duas"
          }]
        }
      },
      "valueCodeableConcept" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoSubstanciaUso",
          "code" : "alcool"
        }]
      },
      "note" : [{
        "text" : "Uso ocasional de cannabis."
      }]
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-10",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-10",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-10\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-10</b></p><a name=\"transient-10\"> </a><a name=\"hctransient-10\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedidaObservada.html\">Medida Observada</a></p></div><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 11885-1}\">11885-1</span></p><p><b>value</b>: 3.5(unit wk from https://www.hl7.org/fhir/valueset-ucum-common.html)<span style=\"background: LightGoldenRodYellow\"> (Detalhes: valueset-ucum-common.html códigowk = 'wk')</span></p></div>"
      },
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "11885-1"
        }]
      },
      "valueQuantity" : {
        "value" : 3.5,
        "system" : "https://www.hl7.org/fhir/valueset-ucum-common.html",
        "code" : "wk"
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-11",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-11",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-11\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-11</b></p><a name=\"transient-11\"> </a><a name=\"hctransient-11\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedidaObservada.html\">Medida Observada</a></p></div><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 9843-4}\">9843-4</span></p><p><b>value</b>: 45.5(unit cm from https://www.hl7.org/fhir/valueset-ucum-common.html)<span style=\"background: LightGoldenRodYellow\"> (Detalhes: valueset-ucum-common.html códigocm = 'cm')</span></p></div>"
      },
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "9843-4"
        }]
      },
      "valueQuantity" : {
        "value" : 45.5,
        "system" : "https://www.hl7.org/fhir/valueset-ucum-common.html",
        "code" : "cm"
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-12",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-12",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada"]
      },
      "text" : {
        "status" : "extensions",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-12\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-12</b></p><a name=\"transient-12\"> </a><a name=\"hctransient-12\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedidaObservada.html\">Medida Observada</a></p></div><p><b>Origem da Medição</b>: <span title=\"Códigos:{http://loinc.org 3138-5}\">Body height Stated</span></p><p><b>Roupas Usadas na Medição</b>: <span title=\"Códigos:{http://loinc.org LA11873-9}\">Street clothes &amp; shoes</span></p><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 29463-7}\">29463-7</span></p><p><b>value</b>: 88.15(unit kg from https://www.hl7.org/fhir/valueset-ucum-common.html)<span style=\"background: LightGoldenRodYellow\"> (Detalhes: valueset-ucum-common.html códigokg = 'kg')</span></p><p><b>method</b>: <span title=\"Códigos:{http://loinc.org LA11870-5}\">Standing</span></p></div>"
      },
      "extension" : [{
        "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BROrigemMedida",
        "valueCodeableConcept" : {
          "coding" : [{
            "system" : "http://loinc.org",
            "code" : "3138-5"
          }]
        }
      },
      {
        "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRRoupasUsadasMedicao",
        "valueCodeableConcept" : {
          "coding" : [{
            "system" : "http://loinc.org",
            "code" : "LA11873-9"
          }]
        }
      }],
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "29463-7"
        }]
      },
      "valueQuantity" : {
        "value" : 88.15,
        "system" : "https://www.hl7.org/fhir/valueset-ucum-common.html",
        "code" : "kg"
      },
      "method" : {
        "coding" : [{
          "system" : "http://loinc.org",
          "code" : "LA11870-5"
        }]
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-13",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-13",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-13\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-13</b></p><a name=\"transient-13\"> </a><a name=\"hctransient-13\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedidaObservada.html\">Medida Observada</a></p></div><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 8480-6}\">8480-6</span></p><p><b>value</b>: 0.15(unit mm[Hg] from https://www.hl7.org/fhir/valueset-ucum-common.html)<span style=\"background: LightGoldenRodYellow\"> (Detalhes: valueset-ucum-common.html códigomm[Hg] = 'mm[Hg]')</span></p><p><b>bodySite</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRLocalAfericao 6}\">Pulso esquerdo</span></p><p><b>method</b>: <span title=\"Códigos:{http://loinc.org LA11868-9}\">Sitting</span></p></div>"
      },
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "8480-6"
        }]
      },
      "valueQuantity" : {
        "value" : 0.15,
        "system" : "https://www.hl7.org/fhir/valueset-ucum-common.html",
        "code" : "mm[Hg]"
      },
      "bodySite" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRLocalAfericao",
          "code" : "6"
        }]
      },
      "method" : {
        "coding" : [{
          "system" : "http://loinc.org",
          "code" : "LA11868-9"
        }]
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-14",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-14",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-14\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-14</b></p><a name=\"transient-14\"> </a><a name=\"hctransient-14\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedidaObservada.html\">Medida Observada</a></p></div><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 11612-9}\">11612-9</span></p><p><b>value</b>: 1</p></div>"
      },
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "11612-9"
        }]
      },
      "valueQuantity" : {
        "value" : 1
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-15",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-15",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-15\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-15</b></p><a name=\"transient-15\"> </a><a name=\"hctransient-15\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedidaObservada.html\">Medida Observada</a></p></div><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 11996-6}\">11996-6</span></p><p><b>value</b>: 2</p></div>"
      },
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "11996-6"
        }]
      },
      "valueQuantity" : {
        "value" : 2
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-16",
    "resource" : {
      "resourceType" : "Observation",
      "id" : "transient-16",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedidaObservada"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Observation_transient-16\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Observation transient-16</b></p><a name=\"transient-16\"> </a><a name=\"hctransient-16\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedidaObservada.html\">Medida Observada</a></p></div><p><b>status</b>: Final</p><p><b>code</b>: <span title=\"Códigos:{https://loinc.org/ 11996-6}\">11996-6</span></p><p><b>value</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoAleitamentoMaterno predominante}\">Predominante</span></p></div>"
      },
      "status" : "final",
      "code" : {
        "coding" : [{
          "system" : "https://loinc.org/",
          "code" : "11996-6"
        }]
      },
      "valueCodeableConcept" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoAleitamentoMaterno",
          "code" : "predominante"
        }]
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-17",
    "resource" : {
      "resourceType" : "AllergyIntolerance",
      "id" : "transient-17",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRAlergiaReacaoAdversa-1.0"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"AllergyIntolerance_transient-17\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: AllergyIntolerance transient-17</b></p><a name=\"transient-17\"> </a><a name=\"hctransient-17\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRAlergiaReacaoAdversa-1.0.html\">Alergia ou Reação Adversa</a></p></div><p><b>clinicalStatus</b>: <span title=\"Códigos:{http://terminology.hl7.org/CodeSystem/allergyintolerance-clinical active}\">Active</span></p><p><b>verificationStatus</b>: <span title=\"Códigos:{http://terminology.hl7.org/CodeSystem/allergyintolerance-verification confirmed}\">Confirmed</span></p><p><b>category</b>: Food</p><p><b>criticality</b>: Low Risk</p><p><b>code</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRImunobiologico 2}\">SAT</span></p><p><b>patient</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0</code>/819217217061851</p><p><b>onset</b>: 2022-06-01</p><p><b>note</b>: </p><blockquote><div><p>Soro antitetânico</p>\n</div></blockquote></div>"
      },
      "clinicalStatus" : {
        "coding" : [{
          "system" : "http://terminology.hl7.org/CodeSystem/allergyintolerance-clinical",
          "code" : "active"
        }]
      },
      "verificationStatus" : {
        "coding" : [{
          "system" : "http://terminology.hl7.org/CodeSystem/allergyintolerance-verification",
          "code" : "confirmed"
        }]
      },
      "category" : ["food"],
      "criticality" : "low",
      "code" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRImunobiologico",
          "code" : "2"
        }],
        "text" : "SAT"
      },
      "patient" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value" : "819217217061851"
        }
      },
      "onsetDateTime" : "2022-06-01",
      "note" : [{
        "text" : "Soro antitetânico"
      }]
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-18",
    "resource" : {
      "resourceType" : "Composition",
      "id" : "transient-18",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRRegistroPrescricaoMedicamento"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Composition_transient-18\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Composition transient-18</b></p><a name=\"transient-18\"> </a><a name=\"hctransient-18\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRRegistroPrescricaoMedicamento.html\">Registro de Prescrição de Medicamento</a></p></div><p><b>status</b>: Final</p><p><b>type</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoDocumento RPM}\">Registro de Prescrição de Medicamento</span></p><p><b>date</b>: 2022-03-04 14:59:51-0300</p><p><b>author</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BREstabelecimentoSaude-1.0</code>/3191384</p><p><b>title</b>: Registro de Prescrição de Medicamento</p></div>"
      },
      "status" : "final",
      "type" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoDocumento",
          "code" : "RPM"
        }]
      },
      "subject" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value" : "819217217061851"
        }
      },
      "date" : "2022-03-04T14:59:51-03:00",
      "author" : [{
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BREstabelecimentoSaude-1.0",
          "value" : "3191384"
        }
      }],
      "title" : "Registro de Prescrição de Medicamento",
      "section" : [{
        "entry" : [{
          "reference" : "urn:uuid:transient-19"
        }]
      }]
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-19",
    "resource" : {
      "resourceType" : "MedicationRequest",
      "id" : "transient-19",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRPrescricaoMedicamento"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"MedicationRequest_transient-19\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: MedicationRequest transient-19</b></p><a name=\"transient-19\"> </a><a name=\"hctransient-19\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRPrescricaoMedicamento.html\">Prescrição de Medicamento</a></p></div><p><b>status</b>: Completed</p><p><b>intent</b>: Order</p><p><b>medication</b>: <a href=\"Bundle-bundle-example-rac-tc.html#urn-uuid-transient-20\">Medication Terminologia segundo CATMAT</a></p><p><b>subject</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0</code>/819217217061851</p><p><b>authoredOn</b>: 2022-03-04</p><p><b>requester</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BREstabelecimentoSaude-1.0</code>/3191384</p><p><b>recorder</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRProfissional-1.0</code>/162338254590005</p><p><b>note</b>: Por Dr. Getúlio @2022-03-04</p><blockquote><div><p>Medicamento necessário para tratamento da febre devido à gripe.</p>\n</div></blockquote><blockquote><p><b>dosageInstruction</b></p><p><b>patientInstruction</b>: Tomar uma vez ao dia via oral.</p><p><b>timing</b>: Contagem 1  times, 12</p><p><b>asNeeded</b>: true</p><p><b>route</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRViaAdministracao 10907}\">Oral</span></p><h3>DoseAndRates</h3><table class=\"grid\"><tr><td style=\"display: none\">-</td><td><b>Type</b></td><td><b>Dose[x]</b></td></tr><tr><td style=\"display: none\">*</td><td><span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRUnidadeMedida 13}\">Cápsula</span></td><td>10</td></tr></table><p><b>maxDosePerAdministration</b>: 10</p></blockquote><h3>DispenseRequests</h3><table class=\"grid\"><tr><td style=\"display: none\">-</td><td><b>ValidityPeriod</b></td><td><b>Quantity</b></td></tr><tr><td style=\"display: none\">*</td><td>2022-02-24 --&gt; 2022-03-03</td><td>10</td></tr></table></div>"
      },
      "status" : "completed",
      "intent" : "order",
      "medicationReference" : {
        "reference" : "urn:uuid:transient-20"
      },
      "subject" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value" : "819217217061851"
        }
      },
      "authoredOn" : "2022-03-04",
      "requester" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BREstabelecimentoSaude-1.0",
          "value" : "3191384"
        }
      },
      "recorder" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRProfissional-1.0",
          "value" : "162338254590005"
        }
      },
      "note" : [{
        "authorString" : "Dr. Getúlio",
        "time" : "2022-03-04",
        "text" : "Medicamento necessário para tratamento da febre devido à gripe."
      }],
      "dosageInstruction" : [{
        "patientInstruction" : "Tomar uma vez ao dia via oral.",
        "timing" : {
          "repeat" : {
            "extension" : [{
              "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRTurno",
              "valueCode" : "3"
            },
            {
              "extension" : [{
                "url" : "periodUnit",
                "valueCode" : "min"
              },
              {
                "url" : "period",
                "valuePositiveInt" : 1
              }],
              "url" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIntervaloDoses"
            }],
            "count" : 1,
            "countMax" : 10,
            "frequency" : 12
          }
        },
        "asNeededBoolean" : true,
        "route" : {
          "coding" : [{
            "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRViaAdministracao",
            "code" : "10907"
          }]
        },
        "doseAndRate" : [{
          "type" : {
            "coding" : [{
              "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRUnidadeMedida",
              "code" : "13"
            }]
          },
          "doseQuantity" : {
            "value" : 10
          }
        }],
        "maxDosePerAdministration" : {
          "value" : 10
        }
      }],
      "dispenseRequest" : {
        "validityPeriod" : {
          "start" : "2022-02-24",
          "end" : "2022-03-03"
        },
        "quantity" : {
          "value" : 10
        }
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-20",
    "resource" : {
      "resourceType" : "Medication",
      "id" : "transient-20",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRMedicamento"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Medication_transient-20\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Medication transient-20</b></p><a name=\"transient-20\"> </a><a name=\"hctransient-20\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRMedicamento.html\">Medicamento</a></p></div><p><b>code</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRObmCATMAT BR0352317}\">Terminologia segundo CATMAT</span></p><p><b>form</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRUnidadeMedida 2}\">Ampola</span></p></div>"
      },
      "code" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRObmCATMAT",
          "code" : "BR0352317"
        }],
        "text" : "Terminologia segundo CATMAT"
      },
      "form" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRUnidadeMedida",
          "code" : "2"
        }]
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-21",
    "resource" : {
      "resourceType" : "CarePlan",
      "id" : "transient-21",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRPlanoCuidados-1.0"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"CarePlan_transient-21\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: CarePlan transient-21</b></p><a name=\"transient-21\"> </a><a name=\"hctransient-21\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRPlanoCuidados-1.0.html\">Plano de Cuidados</a></p></div><p><b>status</b>: Active</p><p><b>intent</b>: Plan</p><p><b>description</b>: Repouso pós-medicação intramuscular</p><p><b>subject</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0</code>/819217217061851</p></div>"
      },
      "status" : "active",
      "intent" : "plan",
      "description" : "Repouso pós-medicação intramuscular",
      "subject" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value" : "819217217061851"
        }
      }
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-22",
    "resource" : {
      "resourceType" : "CarePlan",
      "id" : "transient-22",
      "meta" : {
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRAtestado"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"CarePlan_transient-22\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: CarePlan transient-22</b></p><a name=\"transient-22\"> </a><a name=\"hctransient-22\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\"/><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRAtestado.html\">Atestado Digital</a></p></div><p><b>status</b>: Active</p><p><b>intent</b>: Plan</p><p><b>category</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoDocumento ATM}\">Atestado Médico/Odontológico</span></p><p><b>subject</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0</code>/819217217061851</p><p><b>addresses</b>: <a href=\"Bundle-bundle-example-rac-tc.html#urn-uuid-transient-23\">Condition Varizes esofagianas sem sangramento</a></p><blockquote><p><b>activity</b></p><h3>Details</h3><table class=\"grid\"><tr><td style=\"display: none\">-</td><td><b>Status</b></td><td><b>Scheduled[x]</b></td><td><b>Description</b></td></tr><tr><td style=\"display: none\">*</td><td>Unknown</td><td>Eventos: 2022-07-25 18:11:19+0000 , Contagem 1  times, Uma vez</td><td>Nada digno de nota.</td></tr></table></blockquote></div>"
      },
      "status" : "active",
      "intent" : "plan",
      "category" : [{
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoDocumento",
          "code" : "ATM"
        }]
      }],
      "subject" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value" : "819217217061851"
        }
      },
      "addresses" : [{
        "reference" : "urn:uuid:transient-23"
      }],
      "activity" : [{
        "detail" : {
          "status" : "unknown",
          "scheduledTiming" : {
            "event" : ["2022-07-25T18:11:19.005486Z"],
            "repeat" : {
              "count" : 1
            }
          },
          "description" : "Nada digno de nota."
        }
      }]
    }
  },
  {
    "fullUrl" : "urn:uuid:transient-23",
    "resource" : {
      "resourceType" : "Condition",
      "id" : "transient-23",
      "meta" : {
        "lastUpdated" : "2022-05-09T17:37:55.000322Z",
        "profile" : ["http://www.saude.gov.br/fhir/r4/StructureDefinition/BRCID10Avaliado-1.0"]
      },
      "text" : {
        "status" : "generated",
        "div" : "<div xmlns=\"http://www.w3.org/1999/xhtml\"><a name=\"Condition_transient-23\"> </a><p class=\"res-header-id\"><b>Narrativa gerada: Condition transient-23</b></p><a name=\"transient-23\"> </a><a name=\"hctransient-23\"> </a><div style=\"display: inline-block; background-color: #d9e0e7; padding: 6px; margin: 4px; border: 1px solid #8da1b4; border-radius: 5px; line-height: 60%\"><p style=\"margin-bottom: 0px\">Última atualização: 2022-05-09 17:37:55+0000</p><p style=\"margin-bottom: 0px\">Perfil: <a href=\"StructureDefinition-BRCID10Avaliado-1.0.html\">CID10 Avaliado</a></p></div><p><b>clinicalStatus</b>: <span title=\"Códigos:{http://terminology.hl7.org/CodeSystem/condition-clinical active}\">Active</span></p><p><b>category</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRCategoriaDiagnostico 01}\">Principal</span></p><p><b>code</b>: <span title=\"Códigos:{http://www.saude.gov.br/fhir/r4/CodeSystem/BRCID10 I859}\">Varizes esofagianas sem sangramento</span></p><p><b>subject</b>: Identifier: <code>http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0</code>/819217217061851</p><p><b>note</b>: </p><blockquote><div><p>Varizes esofagianas sem sangramento.</p>\n</div></blockquote></div>"
      },
      "clinicalStatus" : {
        "coding" : [{
          "system" : "http://terminology.hl7.org/CodeSystem/condition-clinical",
          "code" : "active"
        }]
      },
      "category" : [{
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRCategoriaDiagnostico",
          "code" : "01"
        }]
      }],
      "code" : {
        "coding" : [{
          "system" : "http://www.saude.gov.br/fhir/r4/CodeSystem/BRCID10",
          "code" : "I859"
        }]
      },
      "subject" : {
        "identifier" : {
          "system" : "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value" : "819217217061851"
        }
      },
      "note" : [{
        "text" : "Varizes esofagianas sem sangramento."
      }]
    }
  }]
}

```
