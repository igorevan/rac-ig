# O RAC - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## O RAC

### Modelo Computacional

 Para a modelagem do modelo computacional do Registro de Atendimento Clínico (RAC), foram mapeados os campos do Modelo de Informação (MI) aos recursos internacionais [FHIR R4](https://hl7.org/fhir/R4/). Assim, foi realizada a modelagem fechada dos perfis de modo a atender o contexto nacional. 

Foi criado um [Projeto Rede Nacional de Dados em Saúde](https://simplifier.net/redenacionaldedadosemsaude/), na plataforma [SIMPLIFIER.NET](https://simplifier.net/), para a publicação e distribuição dos perfis relacionados aos documentos computacionais em produção na rede.

### Bundle de Envio do RAC

 O diagrama abaixo apresenta o pacote *Bundle* no qual é depositado um Registro de Atendimento Clínico completo, referenciando todos os dados clínicos relevantes para caracterizar um atendimento clínico completo. 

 **Figura 1 - Diagrama do *Bundle* do RAC** 

### Recursos FHIR

 O modelo computacional do RAC, é definido pelo perfil Registro de Atendimento Clínico (`Composition`). 

| | |
| :--- | :--- |
| Composition | ` [ BRRegistroAtendimentoClinico](StructureDefinition-BRRegistroAtendimentoClinico.md) ` |
| Encounter | ` [BRContatoAssistencial](StructureDefinition-BRContatoAssistencial-1.0.md) ` |
| Condition | ` [BRProblemaDiagnostico](StructureDefinition-BRProblemaDiagnostico.md) ` |
| Procedure | ` [BRProcedimentoRealizado](StructureDefinition-BRProcedimentoRealizado-1.0.md) ` |
| Observation | ` [BRMedidaObservada](StructureDefinition-BRMedidaObservada.md) ` |
| AllergyIntolerance | ` [ BRAlergiaReacaoAdversa](StructureDefinition-BRAlergiaReacaoAdversa-1.0.md) ` |
| Composition | ` [ BRRegistroPrescricaoMedicamento](StructureDefinition-BRRegistroPrescricaoMedicamento.md) ` |
| CarePlan | ` [BRPlanoCuidados](StructureDefinition-BRPlanoCuidados-1.0.md) ` |
| CarePlan | ` [BRAtestado](StructureDefinition-BRAtestado.md) ` |
| Location | ` [BRLocalAtendimento](StructureDefinition-BRLocalAtendimento-1.0.md) ` |
| Observation | ` [BRObservacaoDescritiva](StructureDefinition-BRObservacaoDescritiva-1.0.md) ` |
| MedicationRequest | ` [BRPrescricaoMedicamento](StructureDefinition-BRPrescricaoMedicamento.md) ` |
| Medication | ` [BRMedicamento](StructureDefinition-BRMedicamento.md) ` |
| Condition | ` [BRCID10Avaliado](StructureDefinition-BRCID10Avaliado-1.0.md) ` |

Extensões utilizadas:

| | |
| :--- | :--- |
| Extension | ` [BRTurno](StructureDefinition-BRTurno.md) ` |
| Extension | ` [BRRoupasUsadasMedicao](StructureDefinition-BRRoupasUsadasMedicao.md) ` |
| Extension | ` [BRResponsavelAtendimento](StructureDefinition-BRResponsavelAtendimento.md) ` |
| Extension | ` [BRQuantidade](StructureDefinition-BRQuantidade-1.0.md) ` |
| Extension | ` [BROutrasInformacoes](StructureDefinition-BROutrasInformacoes.md) ` |
| Extension | ` [BROrigemMedida](StructureDefinition-BROrigemMedida.md) ` |
| Extension | ` [BROcupacao](StructureDefinition-BROcupacao-1.0.md) ` |
| Extension | ` [BRIntervaloDoses](StructureDefinition-BRIntervaloDoses.md) ` |
| Extension | ` [ BRIndividuoNaoIdentificado](StructureDefinition-BRIndividuoNaoIdentificado-1.0.md) ` |
| Extension | ` [BRIdentificacaoEquipe](StructureDefinition-BRIdentificacaoEquipe-1.0.md) ` |
| Extension | ` [BRFinanciamento](StructureDefinition-BRFinanciamento-1.0.md) ` |
| Extension | ` [BRCodigoSerialMedicamento](StructureDefinition-BRCodigoSerialMedicamento.md) ` |

Perfis dos tipos *ValueSet* e *CodeSystem* estão associados a recursos terminológicos. No contexto de Atendimento Clínico e os domínios utilizados, foram criados * CodeSystems* específicos definidos pelo [Comitê Gestor de Saúde Digital (CGSD)](https://www.gov.br/saude/pt-br/acesso-a-informacao/participacao-social/conselhos-e-orgaos-colegiados/cgsd).

Vale destacar que os perfis terminológicos podem passar por atualizações e versionamentos com periodicidade específica de cada domínio, por isso é importante acompanhar a disponibilização dessas atualizações no projeto [RNDS no Simplifier](https://simplifier.net/redenacionaldedadosemsaude). 

Note que na estrutura dos perfis há elementos com bindings para *ValueSets* que apontam para *CodeSystems*. Já no JSON (`Bundle`), o elemento “*system*” sempre indicará os *CodeSystems* relacionados aos códigos (“*value*”) indicados pelo integrador (autor do registro). 

| | |
| :--- | :--- |
| [ RoupasUsadasMedicao](https://simplifier.net/redenacionaldedadosemsaude/valueset-brroupasusadasmedicao) | [LOINC](http://loinc.org) |
| [ BRViaAdministracao](https://simplifier.net/redenacionaldedadosemsaude/valueset-brviaadministracao-1.0) | [ BRViaAdministracao](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brviaadministracao) |
| [ BRUnidadeTempo](https://simplifier.net/redenacionaldedadosemsaude/valueset-brunidadetempo) | [ BRUnidadeTempo](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brunidadetempo) |
| [ BRUnidadeMedidaMedicamento](https://simplifier.net/redenacionaldedadosemsaude/valueset-brunidademedidamedicamento) | [ BRUnidadeMedida](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brunidademedida) |
| [ BRUnidadeConsumo](https://simplifier.net/redenacionaldedadosemsaude/valueset-brunidadeconsumo) | |
| [BRTurno](https://simplifier.net/redenacionaldedadosemsaude/valueset-brturno) | [BRTurno](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brturno) |
| [ BRTipoAleitamentoMaterno](https://simplifier.net/redenacionaldedadosemsaude/valueset-brtipoaleitamentomaterno-1.0) | [ BRTipoAleitamentoMaterno](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brtipoaleitamentomaterno) |
| [ BRTipoObservacao](https://simplifier.net/redenacionaldedadosemsaude/valueset-brtipoobservacao-1.0) | [ BRTabelaSUS](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brtabelasus) |
| [ BRTipoObservacao](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brtipoobservacao) | |
| [ BRTipoIdentificadorProcedimento](https://simplifier.net/redenacionaldedadosemsaude/valueset-brtipoidentificadorprocedimento-1.0) | [ BRTipoIdentificador](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brtipoidentificador) |
| [ BRTipoDocumento](https://simplifier.net/redenacionaldedadosemsaude/valueset-brtipodocumento-1.0) | [ BRTipoDocumento](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brtipodocumento) |
| [ BRTerminologiaMedicamento](https://simplifier.net/redenacionaldedadosemsaude/valueset-brterminologiamedicamento) | [ BRObmCATMAT](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brobmcatmat) |
| [BRObmEAN](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brobmean) | |
| [ BRObmANVISA](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brobmanvisa) | |
| [BRObmAMPP](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brobmampp) | |
| [ BRResponsabilidadeParticipante](https://simplifier.net/redenacionaldedadosemsaude/valueset-brresponsabilidadeparticipante-1.0) | [ BRResponsabilidadeParticipante](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brresponsabilidadeparticipante) |
| [ BRProcedimentosNacionais](https://simplifier.net/redenacionaldedadosemsaude/valueset-brprocedimentosnacionais-1.0) | [ BRCBHPMTUSS](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brcbhpmtuss) |
| [ BRTabelaSUS](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brtabelasus) | |
| [ BRProcedencia](https://simplifier.net/redenacionaldedadosemsaude/valueset-brprocedencia-1.0) | [ BRProcedencia](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brprocedencia) |
| [ BRPosicaoIndividuo](https://simplifier.net/redenacionaldedadosemsaude/valueset-brposicaoindividuo) | [ BRPosicaoIndividuo](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brposicaoindividuo) |
| [ BROrigemMedida](https://simplifier.net/redenacionaldedadosemsaude/valueset-brorigemmedida) | [LOINC]() |
| [ BROcupacao](https://simplifier.net/redenacionaldedadosemsaude/valueset-brocupacao-1.0) | [BRCBO](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brcbo) |
| [ BRMotivoDesfechoDocumentos](https://simplifier.net/redenacionaldedadosemsaude/valueset-brmotivodesfechodocumentos-1.0) | [ BRMotivoDesfecho](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brmotivodesfecho) |
| [ BRMotivoDesfecho](https://simplifier.net/redenacionaldedadosemsaude/valueset-brmotivodesfecho-1.0) | |
| [ BRModalidadeFinanceira](https://simplifier.net/redenacionaldedadosemsaude/valueset-brmodalidadefinanceira) | [ BRModalidadeFinanceira](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brmodalidadefinanceira) |
| [ BRModalidadeAssistencial](https://simplifier.net/redenacionaldedadosemsaude/valueset-brmodalidadeassistencial-1.0) | [ BRModalidadeAssistencial](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brmodalidadeassistencial) |
| [ BRLocalAtendimento](https://simplifier.net/redenacionaldedadosemsaude/valueset-brlocalatendimento-1.0) | [ BRLocalAtendimento](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brlocalatendimento) |
| [ BRLocalAfericao](https://simplifier.net/redenacionaldedadosemsaude/valueset-brlocalafericao-1.0) | [ BRLocalAfericao](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brlocalafericao) |
| [ BRImunobiologico](https://simplifier.net/redenacionaldedadosemsaude/valueset-brimunobiologico-1.0) | [ BRImunobiologico](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brimunobiologico) |
| [ BRGrauCertezaAlergiasReacoesAdversas](https://simplifier.net/redenacionaldedadosemsaude/valueset-brgraucertezaalergiasreacoesadversas-1.0) | [ allergyintolerance-verification](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/80047) |
| [ BRFrequenciaUsoSubstancia](https://simplifier.net/redenacionaldedadosemsaude/valueset-brfrequenciausosubstancia) | [ v3-GTSAbbreviation](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/79475) |
| [ BRFinanciamento](https://simplifier.net/redenacionaldedadosemsaude/valueset-brfinanciamento-1.0) | [ BRFinanciamento](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brfinanciamento) |
| [ BREstadoSolicitacao](https://simplifier.net/redenacionaldedadosemsaude/valueset-brestadosolicitacaomedicamento-1.0) | [ request-status](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/83465) |
| [ BREstadoResolucaoDiagnosticoProblema](https://simplifier.net/redenacionaldedadosemsaude/valueset-brestadoresolucaodiagnosticoproblema-1.0) | [ condition-clinical](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/79466) |
| [ BREstadoObservacao](https://simplifier.net/redenacionaldedadosemsaude/valueset-brestadoobservacao-1.0) | [ observation-status](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/78899) |
| [ BREstadoEvento](https://simplifier.net/redenacionaldedadosemsaude/valueset-brestadoevento-1.0) | [event-status](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/80010) |
| [ BREstadoDocumento](https://simplifier.net/redenacionaldedadosemsaude/valueset-brestadodocumento-1.0) | [ composition-status](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/80407) |
| [ BREstadoContatoAssistencial](https://simplifier.net/redenacionaldedadosemsaude/valueset-brestadocontatoassistencial-1.0) | [ encounter-status](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/80025) |
| [ BRCriticidadeAlergiasReacoesAdversas](https://simplifier.net/redenacionaldedadosemsaude/valueset-brcriticidadealergiasreacoesadversas-1.0) | [allergy-intolerance-criticality]() |
| [ BRCategoriaDiagnostico](https://simplifier.net/redenacionaldedadosemsaude/valueset-brcategoriadiagnostico) | [ BRCategoriaDiagnostico](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brcategoriadiagnostico) |
| [ BRCategoriaAgenteAlergiasReacoesAdversas](https://simplifier.net/redenacionaldedadosemsaude/valueset-brcategoriaagentealergiasreacoesadversas-1.0) | [ allergy-intolerance-category](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/81870) |
| [ BRCaraterAtendimento](https://simplifier.net/redenacionaldedadosemsaude/valueset-brcarateratendimento-1.0) | [ BRCaraterAtendimento](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brcarateratendimento) |
| [BRCID10](https://simplifier.net/redenacionaldedadosemsaude/valueset-brcid10-1.0) | [BRCID10](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brcid10) |
| [ BRAlergenos](https://simplifier.net/redenacionaldedadosemsaude/valueset-bralergenos-1.0) | [ BRAlergenosCBARA](https://simplifier.net/redenacionaldedadosemsaude/codesystem-bralergenoscbara) |
| [ BRImunobiologico](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brimunobiologico) | |
| [ BRMedicamento](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brmedicamento) | |
| [ BRTipoAtestado](https://simplifier.net/redenacionaldedadosemsaude/valueset-brtipoatestado) | [ BRTipoDocumento](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brtipodocumento) |
| [ BREstadoAfastamentoAtestado](https://simplifier.net/redenacionaldedadosemsaude/valueset-brestadoafastamentoatestado) | [ care-plan-activity-status](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/83364) |
| [ BRIntencaoAtestado](https://simplifier.net/redenacionaldedadosemsaude/valueset-brintencaoatestado) | [ request-intent](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/81826) |
| [ BREstadoAtestado](https://simplifier.net/redenacionaldedadosemsaude/valueset-brestadoatestado) | [ request-status](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/83465) |
| [ BRPapelProblemaDiagnostico](https://simplifier.net/redenacionaldedadosemsaude/valueset-brpapelproblemadiagnostico) | [ BRPapelProblemaDiagnostico](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brpapelproblemadiagnostico) |
| [ diagnosis-role](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/83484) | |
| [ BREstadoResolucaoDiagnosticoProblema](https://simplifier.net/redenacionaldedadosemsaude/valueset-brestadoresolucaodiagnosticoproblema-1.0) | [ condition-clinical](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/79466) |
| [ BRCategoriaCondicao](https://simplifier.net/redenacionaldedadosemsaude/valueset-brcategoriacondicao) | [ condition-category](https://simplifier.net/packages/hl7.fhir.r4.core/4.0.1/files/79008) |
| [ BRProblemaDiagnostico](https://simplifier.net/redenacionaldedadosemsaude/valueset-brproblemadiagnostico) | [BRCID10](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brcid10) |
| [BRCIAP2](https://simplifier.net/redenacionaldedadosemsaude/codesystem-brciap2) | |

