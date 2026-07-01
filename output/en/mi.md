# Modelo de Informação - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## Modelo de Informação

### Objetivo

O RAC tem como objetivo estabelecer especificações de informações promovendo um padrão único de consenso nacional e possibilitando a interoperabilidade dos dados em saúde, essenciais entre os provedores de cuidados em saúde. 

O RAC vai atuar nos níveis da Atenção Primária em Saúde e na atenção especializada, contribuindo para uma atenção coordenada entre os cuidadores e apoiando na continuidade do cuidado ao indivíduo em âmbito laboratorial. 

### Público-alvo

Público-alvo proposto pelo RAC:

* Profissionais de saúde (que acompanham regularmente o indivíduo e os que venham a atendê-lo em situações de urgência/emergência ou fora de seu atendimento de rotina);
* Estabelecimentos de saúde em fase de planejamento e implementação ou melhorias de seus sistemas de informação e saúde, visando a interoperabilidade;
* Vendedores e desenvolvedores de software;
* Gestores e realizadores de políticas públicas, especialistas clínicos, gerentes de informática em saúde e equipes de suporte, bem como integradores de sistemas;
* Usuários dos serviços de saúde e suas entidades representativas;
* Especialistas responsáveis apenas por algum aspecto específico da saúde do indivíduo, tais como diabetes ou gravidez e,
* O próprio indivíduo e ou seus responsáveis.

### Marcos Legais

*  [Portaria no. 234 de 18 de julho de 2022](https://www.in.gov.br/en/web/dou/-/portaria-n-234-de-18-de-julho-de-2022-416506215) 
*  [ https://rnds-guia.saude.gov.br/docs/rac/mi-rac ](https://rnds-guia.saude.gov.br/docs/rac/mi-rac ) 

### Modelo de Informação

 O modelo de informação é uma representação conceitual e canônica, onde os elementos referentes a um documento específico são modelados em seções e blocos de dados, com seus respectivos tipos de dados a serem informados. Também são apresentadas as referências para o uso de recursos terminológicos, da seguinte maneira: 

*  **Coluna 1** - Nível: apresenta o nível do elemento no modelo de informação; 
* **Coluna 2** - Cardinalidade: descreve o número de vezes que o elemento deve/pode aparecer:
*  **Coluna 3** - Seção/item: nome do bloco ou da informação a ser enviada; 
*  **Coluna 4** - Tipo de dado: descreve o tipo de dado a ser preenchido; 
*  **Coluna 5** - Conceitos/Observações (Regra de negócio): apresenta o conceito e/ou a regra referente ao elemento; 
*  **Coluna 6** - Recurso FHIR: relaciona os atributos do modelo informacional com os atributos dos artefatos computacionais 

### Blocos do Modelo de Informação

 Segue abaixo o modelo de informação para o Registro de Atendimento Clínico: 

#### Identificação do Indivíduo

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [1..1] | Identificação do indivíduo | Seção | RN01: O documento deve trazer um identificador nacional do indíviduo. Se não houver nenhum dos dois possíveis (CNS ou CPF), dever ser obrigatório o preenchimento do bloco Identificação por dados demográficos. |  |  |
| 2 | [1..1] | Identificador Nacional do Indivíduo | Caracteres numéricos | Identificação unívoca dos usuários das ações e serviços de saúde, mediante número único válido em todo o território nacional, sendo: Cartão Nacional de Saúde (CNS); Cadastro de Pessoa Física (CPF). RN01: A validação do identificador nacional do indivíduo deve ser feita junto ao CADSUS. RN02: Se o campo vier preenchido com CPF e o indivíduo não possuir CNS correspondente, necessita ser criado. |  | Indivíduo |
| 2 | [0..1] | Identificação por dados demográficos |  | RN03: Na hipótese de não ser possível a identificação por um dos identificadores nacionais acima, os campos do bloco de dados demográficos serão usados como parâmetros de pesquisa para a identificação do indivíduo e eventual atribuição de um CNS. |  | [Informações Complementares de Indivíduos Não Identificados](StructureDefinition-BRIndividuoNaoIdentificado-1.0.md) |
| 3 | [1..1] | Nome completo | Sequência de caracteres alfanuméricos |  |  | Indivíduo |
| 3 | [0..1] | Nome social | Sequência de caracteres alfanuméricos |  |  | Indivíduo |
| 3 | [1..1] | Nome completo da mãe | Sequência de caracteres alfanuméricos |  |  | Indivíduo |
| 3 | [1..1] | Data de nascimento | Data | Conforme ISO 8601. |  | Indivíduo |
| 3 | [1..1] | Sexo | Texto codificado | Masculino, Feminino, Ignorado |  | Indivíduo |
| 3 | [0..1] | País de nascimento | Texto codificado | RN04: Obrigatório se país estrangeiro. |  | Indivíduo |
| 3 | [0..1] | Município de Nascimento | Texto codificado | RN05: Preenchido somente se o país de nascimento for Brasil. |  | Indivíduo |
| 2 | [0..1] | Endereço | Sequência de caracteres alfanuméricos | RN06: Preenchido somente se o país de nascimento for Brasil. |  | Indivíduo |

#### Caracterização do Atendimento

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [1..1] | Caracterização do atendimento |  |  |  |  |
| 2 | [1..1] | Identificador do Estabelecimento de saúde | Caracteres numéricos | Identificação unívoca do estabelecimento de atendimento, mediante número único válido em todo o território nacional, sendo: - Cadastro Nacional de Estabelecimentos de Saúde (CNES). |  | [Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md) |
| 2 | [1..1] | Procedência | Texto codificado: Ordem Judicial, Retorno, Demanda espontânea, Demanda Referenciada | Identifica o serviço que encaminhou o indivíduo ou a sua iniciativa/de seu responsável na busca pelo acesso ao serviço de saúde. | [Procedência](ValueSet-BRProcedencia-1.0.md) | [Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md) |
| 2 | [0..1] | Identificação da equipe de saúde | Caracteres numéricos. | Número válido do Identificador Nacional de Equipe (INE) no CNES. |  | [Identificador Nacional de Equipe](StructureDefinition-BRIdentificacaoEquipe-1.0.md), presente em[Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md) |
| 2 | [1..1] | Data e hora do atendimento | Data e hora | Conforme ISO 8601. Data e hora da aceitação do indivíduo para início do atendimento. |  | [Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md) |
| 2 | [1..1] | Modalidade assistencial | Texto codificado: Atenção Básica, Ambulatorial Especializada, Atenção Domiciliar, Atenção Psicossocial, Atenção à Urgência/Emergência | Classificação do contato com o serviço de saúde de acordo com as especificidades do modo, local e duração do atendimento. | [Modalidade Assistencial](ValueSet-BRModalidadeAssistencial-1.0.md) | [Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md) |
| 2 | [1..1] | Caráter de atendimento | Texto codificado: Consulta agendada, Consulta agendada programada: cuidado continuado, Demanda espontânea (DE): consulta no dia, Demanda espontânea (DE): atendimento de urgência | Identifica o contato assistencial de acordo com a prioridade de sua realização. | [Caráter de atendimento do Contato Assistencial](ValueSet-BRCaraterAtendimento-1.0.md) | [Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md) |
| 2 | [1..1] | Profissionais do atendimento |  |  |  | Profissional |
| 3 | [1..N] | Profissional |  |  |  | Profissional |
| 4 | [0..1] | Nome do profissional | Texto livre |  |  | Profissional |
| 4 | [1..1] | Número do conselho do profissional atendente | Caracteres numéricos | Indica o número do conselho do profissional atendente |  | Profissional |
| 4 | [1..1] | Conselho do profissional atendente | Texto Codificado | Indica a entidade de conselho do profissional atendente (CRM, CRF, CRO, ...) |  | Profissional |
| 4 | [1..1] | UF do conselho do profissional atendente | Texto Codificado | Indica a UF do Conselho do Profissional atendente |  | Profissional |
| 3 | [1..1] | Identificador do profissional atendente | Caracteres numéricos | Identificação unívoca do profissional prescritor, mediante número único válido em todo o território nacional, sendo: Cadastro de Pessoa Física (CPF). RN08: Validar junto ao CADSUS. |  | Profissional |
| 4 | [1..1] | Ocupação do profissional | Texto codificado por terminologia externa: CBO | Atividade desempenhada pelo profissional que realizou o atendimento. | [Classificação Brasileira de Ocupações - CBO](ValueSet-BROcupacao-1.0.md) | [Ocupação](StructureDefinition-BROcupacao-1.0.md), presente em[Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md) |
| 4 | [1..1] | É o responsável pelo atendimento? | Texto codificado: Sim, Não |  |  | [Responsável pelo Atendimento](StructureDefinition-BRResponsavelAtendimento.md), presente em[Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md) |

#### Motivo do Atendimento Estruturado

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [0..1] | Motivo do atendimento estruturado |  |  |  |  |
| 2 | [0..N] | Motivo do atendimento estruturado |  |  |  |  |
| 3 | [1..1] | Terminologia que descreve o motivo do atendimento | Texto codificado: CID, CIAP | Identificador da terminologia que será utilizada para descrever o motivo de atendimento. |  | [Problema / Diagnóstico](StructureDefinition-BRProblemaDiagnostico.md) |
| 3 | [1..1] | Código do motivo do atendimento | Texto codificado por terminologia externa: CID-9, CID-10, CID-11, CIAP-1, CIAP-2 |  | [Classificação Internacional de Doenças e Atenção Primária](ValueSet-BRProblemaDiagnostico.md) | [Problema / Diagnóstico](StructureDefinition-BRProblemaDiagnostico.md) |
| 2 | [0..1] | Declaração subjetiva do indivíduo para o atendimento | Texto livre |  |  | [Observação Descritiva](StructureDefinition-BRObservacaoDescritiva-1.0.md) |

#### Observações

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [0..1] | Observações |  |  |  |  |
| 2 | [0..1] | Sinais vitais |  |  |  | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Pressão Arterial |  |  |  | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [1..1] | Sistólica | Caracteres numéricos |  | Quantidade indicada de 0 a 1000 | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [1..1] | Unidade de medida da Pressão arterial Sistólica | Texto codificado |  | mmHg | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [1..1] | Diastólica | Caracteres numéricos |  | Quantidade indicada de 0 a 1000 | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [1..1] | Unidade de medida da Pressão arterial Diastólica | Texto codificado |  | mmHg | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [0..1] | Posição do indivíduo na aferição | Texto codificado: Em pé, Sentado, Reclinado, Deitado, Deitado com inclinação para esquerda | Indica a posição do indivíduo no momento da aferição da pressão arterial. | [Posição do Indivíduo](ValueSet-BRPosicaoIndividuo.md) | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [0..1] | Local de aferição | Texto codificado: Braço direito, Braço esquerdo, Coxa direita, Coxa esquerda, Pulso direito, Pulso esquerdo, Tornozelo direito, Tornozelo esquerdo, Dedo da mão, Dedo do pé | Identifica qual parte do corpo humano foi utilizada para aferir a pressão arterial. | [Local de Aferição](ValueSet-BRLocalAfericao-1.0.md) | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 2 | [0..1] | Medições |  |  |  | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Peso | Caracteres numéricos | Tipo de mensuração | Quantidade indicada de 0 a 1000 | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [1..1] | Unidade de medida do peso | Texto codificado pelo HL7 FHIR (http://hl7.org/fhir/ValueSet/ucum-bodyweight): kg, lb_av, g | Unidade de medida do peso utilizada para medição. | Kg, g | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Posição em relação à gravidade | Texto codificado: LOINC - https://loinc.org/8361-8/ e https://loinc.org/8352-7 | De acordo com lista LOINC de padronização de informação, determinar como a mensuração foi realizada: De pé, Deitado, Sentado | [Posição do Indivíduo](ValueSet-BRPosicaoIndividuo.md) | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Roupas usadas durante a medição | Texto codificado: loinc.org/8352-7 | De acordo com lista LOINC de padronização de informação, determinar como a mensuração foi realizada (roupas usadas durante a medição): Roupa íntima ou menos; Roupas de rua, sem sapatos; Roupas e sapatos de rua | [Roupas Usadas na Medição](ValueSet-RoupasUsadasMedicao.md) | [Roupas Usadas na Medição](StructureDefinition-BRRoupasUsadasMedicao.md), presente em[Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [1..1] | Origem da medição | Texto codificado: Medido (3141-9), Relatado (3142-7) | Informar se o peso foi aferido no atendimento ou relatado. | [Origem de Medição](ValueSet-BROrigemMedida.md) | [Origem da Medição](StructureDefinition-BROrigemMedida.md), presente em[Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Altura | Caracteres numéricos |  | Quantidade indicada de 0 a 1000 | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [1..1] | Unidade de medida da altura | Texto codificado: http://hl7.org/fhir/ValueSet/ucum-bodylength | Unidade de medida da altura utilizada para medição da altura | cm | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [0..1] | Posição em relação à gravidade | Texto codificado: LOINC - https://loinc.org/8361-8/ | De acordo com lista LOINC de padronização de informação, determinar como a mensuração foi realizada: De pé, Deitado, Sentado | [Posição do Indivíduo](ValueSet-BRPosicaoIndividuo.md) | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [0..1] | Origem da medição | Texto codificado (https://loinc.org/3138-5): Medido (3137-7), Relatado (3138-5) | Informar se a altura foi aferido no atendimento ou relatado. | [Origem de Medição](ValueSet-BROrigemMedida.md) | [Origem da Medição](StructureDefinition-BROrigemMedida.md), presente em[Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Perímetro cefálico | Caracteres numéricos |  | Quantidade indicada de 0 a 100 | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [1..1] | Unidade de medida do perímetro cefálico | Texto codificado: http://hl7.org/fhir/ValueSet/ucum-bodylength | Unidade de medida utilizada para medição do perímetro cefálico | cm | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Circunferência abdominal | Caracteres numéricos |  | Quantidade indicada em cm | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [1..1] | Unidade de medida da Circunferência Abdominal | Texto codificado: https://loinc.org/8281-8/ | Unidade de medida utilizada para medição da Circunferência Abdominal | cm | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 2 | [0..1] | Informações adicionais | Texto livre |  |  | [Observação Descritiva](StructureDefinition-BRObservacaoDescritiva-1.0.md) |
| 3 | [0..1] | DUM (Data da Última Menstruação) | Data | Conforme ISO 8601 |  | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Idade gestacional | Caracteres numéricos |  | Quantidade indicada em dias ou semanas | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [1..1] | Unidade de medida da Idade Gestacional | Texto codificado | Unidade de medida de tempo usada no campo Idade Gestacional | dias ou semanas gestacionais | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Quantidade de gestas prévias | Caracteres numéricos |  | Quantidade indicada de 0 a 99 | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Quantidade de Partos | Caracteres numéricos |  | Quantidade indicada de 0 a 99 | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Quantidade de Abortos | Caracteres numéricos |  | Quantidade indicada de 0 a 99 | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..1] | Tipo de aleitamento materno para crianças até 2 anos | Texto Codificado: Exclusivo, Predominante, Complementado, Inexistente |  | [Tipo de Aleitamento Materno](ValueSet-BRTipoAleitamentoMaterno-1.0.md) | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 3 | [0..N] | Exposição à substâncias |  |  |  | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 4 | [0..N] | Uso de álcool, tabaco e outras substâncias nos últimos 3 meses |  |  |  | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 5 | [0..1] | Substância | Texto codificado |  | [Tipo de Substância em Uso](ValueSet-BRTipoSubstanciaUso-1.0.md) | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 5 | [0..1] | Outras substâncias não especificadas | Texto livre |  |  | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |
| 5 | [0..1] | Frequência nos últimos 3 meses | Texto codificado: Nunca, Mensalmente, 2 ou mais vezes ao mês, Semanalmente, Diariamente ou quase todos os dias |  | [Frequência de Uso da Substância](ValueSet-BRFrequenciaUsoSubstancia.md) | [Medida Observada](StructureDefinition-BRMedidaObservada.md) |

#### Problemas/Diagnósticos Avaliados

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [1..N] | Problemas / diagnósticos avaliados |  | Informações sobre a condição de saúde, lesão, deficiência ou qualquer outra questão que afete o bem-estar físico, mental ou social de um indivíduo. Identificadas em um contato assistencial. Para fins de documentação clínica com este dado, o problema e o diagnóstico são considerados como um continuum, com níveis crescentes de detalhes e evidências de suporte geralmente fornecendo peso para o rótulo de 'diagnóstico'. Nesse campo, não é necessário classificar a condição como 'problema' ou 'diagnóstico' (Adaptado do conceito de Problema/Diagnóstico do Clinical Knowledge Manager/OpenEHR). |  |  |
| 2 | [1..1] | Código do diagnóstico/Problema | Texto codificado por terminologia externa | Código do Diagnóstico/Problema detectado (ex: Z47, M52.3, ...) | [Classificação Internacional de Doenças e Atenção Primária](ValueSet-BRProblemaDiagnostico.md) | [Problema / Diagnóstico](StructureDefinition-BRProblemaDiagnostico.md) |
| 2 | [1..1] | Terminologia que descreve o diagnóstico / problema | Texto codificado: CID, CIAP | Identificador da terminologia que será utilizada para informar os problemas/diagnósticos avaliados. |  | [Problema / Diagnóstico](StructureDefinition-BRProblemaDiagnostico.md) |
| 2 | [0..1] | Categoria do diagnóstico | Texto Codificado: Principal, Secundário | Condição estabelecida após estudo de forma a esclarecer qual o mais importante ou principal motivo responsável pela demanda do contato assistencial. O diagnóstico primário reflete achados clínicos descobertos durante a permanência do indivíduo no estabelecimento de saúde, podendo, portanto, ser diferente do diagnóstico de admissão (Port. nº 1.324/SAS/MS/2014) | [Categoria do Diagnóstico](ValueSet-BRCategoriaDiagnostico.md) | [CID10 Avaliado](StructureDefinition-BRCID10Avaliado-1.0.md) |
| 2 | [0..1] | Estado de resolução do problema | Texto codificado: Ativo, Recorrente, Recidiva, Inativo, Remissão, Resolvido |  | [Estado da Resolução de Diagnóstico ou Problema](ValueSet-BREstadoResolucaoDiagnosticoProblema-1.0.md) | [Problema / Diagnóstico](StructureDefinition-BRProblemaDiagnostico.md) |
| 2 | [0..1] | Nota | Texto livre |  |  | [Problema / Diagnóstico](StructureDefinition-BRProblemaDiagnostico.md) |

#### Alergia e/ou Reação Adversa

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [0..N] | Alergia e/ou reação adversa |  | Reatividade alterada a um antígeno pode resultar em reações patológicas consequentes à exposição subsequente àquele antígeno particular. |  |  |
| 2 | [1..1] | Categoria do agente causador da alergia ou reação adversa | Texto codificado: Alimento, Medicamento, Biológica, Outras substâncias, Fator Externo/Ambiental |  | [Categoria do Agente da Alergia ou Reação Adversa](ValueSet-BRCategoriaAgenteAlergiasReacoesAdversas-1.0.md) | [Alergia ou Reação Adversa](StructureDefinition-BRAlergiaReacaoAdversa-1.0.md) |
| 2 | [1..1] | Agente/substância específica | Texto dodificado: CBARA, CATMAT, Lista de vacinas do PNI |  | [Alérgenos](ValueSet-BRAlergenos-1.0.md) | [Alergia ou Reação Adversa](StructureDefinition-BRAlergiaReacaoAdversa-1.0.md) |
| 2 | [0..1] | Manifestação | Texto codificado: CBARA |  | [Reações Adversas da MedDRA](ValueSet-BRReacoesAdversasMedDRA-1.0.md) | [Alergia ou Reação Adversa](StructureDefinition-BRAlergiaReacaoAdversa-1.0.md) |
| 2 | [0..1] | Grau de certeza | Texto codificado: Não Confirmada, Confirmada, Refutada, Cancelada por informação errada |  | [Grau de Certeza de Alergias e Reações Adversas](ValueSet-BRGrauCertezaAlergiasReacoesAdversas-1.0.md) | [Alergia ou Reação Adversa](StructureDefinition-BRAlergiaReacaoAdversa-1.0.md) |
| 2 | [0..1] | Criticidade | Texto codificado: Baixa, Alta, Inderteminada | Uma indicação do potencial de danos nos órgãos críticos do sistema ou consequência de ameaça à vida. | [Criticidade de Alergias e Reações Adversas](ValueSet-BRCriticidadeAlergiasReacoesAdversas-1.0.md) | [Alergia ou Reação Adversa](StructureDefinition-BRAlergiaReacaoAdversa-1.0.md) |
| 2 | [0..1] | Data da instalação da reação adversa | Data |  | Conforme ISO 8601 | [Alergia ou Reação Adversa](StructureDefinition-BRAlergiaReacaoAdversa-1.0.md) |
| 2 | [0..1] | Evolução da alergia/reação adversa | Texto livre |  |  | [Alergia ou Reação Adversa](StructureDefinition-BRAlergiaReacaoAdversa-1.0.md) |

#### Procedimento(s) Realizado(s) ou Solicitado(s)

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [0..N] | Procedimento (s) realizado (s) ou solicitado (s) |  |  |  |  |
| 2 | [1..1] | Terminologia que descreve o procedimento | Texto codificado: SIGTAP, CBHPM ou TUSS | Identificador único do Objeto: identificador da terminologia que será utilizada para informar procedimento(s) realizado(s) ou solicitado(s). |  | [Procedimento Realizado](StructureDefinition-BRProcedimentoRealizado-1.0.md) |
| 3 | [1..1] | Nome do procedimento | Texto codificado por terminologia externa: SIGTAP, CBHPM ou TUSS | Ação de saúde realizada no indivíduo durante o contato assistencial (Ex: Número TUSS). | [Procedimento realizado](ValueSet-BRProcedimentosNacionais-1.0.md) | [Procedimento Realizado](StructureDefinition-BRProcedimentoRealizado-1.0.md) |
| 3 | [1..1] | Status do procedimento | Texto codificado: Pré-procedimento, Em andamento, Não Realizado, Suspenso, Cancelado, Completado, Desconhecido, Entrada com erro. | Mais usado para procedimentos médicos de saúde | [Estado do Evento](ValueSet-BREstadoEvento-1.0.md) | [Procedimento Realizado](StructureDefinition-BRProcedimentoRealizado-1.0.md) |
| 3 | [0..1] | Resultado ou observações do procedimento | Texto livre |  |  | [Procedimento Realizado](StructureDefinition-BRProcedimentoRealizado-1.0.md) |

#### Prescrição no Atendimento

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [1..1] | Prescrição no atendimento | Seção |  |  | [Registro de Prescrição de Medicamento](StructureDefinition-BRRegistroPrescricaoMedicamento.md) |
| 2 | [0..1] | Medicamentos prescritos no atendimento (não estruturado) |  |  |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 3 | [1..1] | Descrição da prescrição | Texto livre | Descrição da prescrição de medicamentos de forma livre, em texto, podendo ter vários medicamentos no mesmo texto. O profissional prescritor deverá descrever todos os campos necessários a uma prescrição, entre outros elementos relevantes. |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 2 | [0..1] | Medicamentos prescritos no atendimento (estruturado) |  |  |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 3 | [1..1] | Terminologia que descreve o medicamento | Texto codificado | Lista de registro de medicamentos da ANVISA Ontologia Brasileira em Saúde (OBS), Catálogo de Materiais do Governo Federal (CATMAT) |  | [Medicamento](StructureDefinition-BRMedicamento.md) |
| 4 | [1..N] | Medicamento | Texto codificado por terminologia externa | Indica o nome do princípio ativo, concentração, unidade de medida e forma farmacêutica do medicamento prescrito. | [Terminologia dos medicamentos](ValueSet-BRTerminologiaMedicamento.md) | [Medicamento](StructureDefinition-BRMedicamento.md) |
| 5 | [1..1] | Via de administração | Texto codificado por terminologia externa |  | [Via de Administração do Imunobiológico](ValueSet-BRViaAdministracao-1.0.md) | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 5 | [1..1] | Posologia |  |  |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 6 | [0..1] | Posologia não estruturada | Texto livre | Descrição da posologia de medicamento de forma livre, em texto. O profissional prescritor deverá descrever todos os campos necessários a uma posologia, entre outros elementos relevantes. |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 6 | [0..1] | Posologia estruturada |  |  |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 7 | [1..1] | Quantidade da Dose | Caracteres numéricos | Quantidade da unidade de consumo do medicamento prescrito a cada dose. |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 7 | [1..1] | Unidade de consumo da dose | Texto codificado por terminologia externa | Unidade de consumo do medicamento prescrito (ex.: comprimido, cápsula, aplicação, mL, gota, copo dosador, infusão, etc.) | [Unidade de Consumo](ValueSet-BRUnidadeConsumo.md) | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 7 | [1..1] | Frequência de uso do medicamento |  |  |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 8 | [1..1] | Dose única | Boleano |  | Verdadeiro, Falso | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 8 | [0..1] | Uso contínuo |  | RN09: preenchido obrigatoriamente se "Dose Única" = não/falso |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 7 | [0..1] | Quantidade de medicamento prescrito |  |  |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 8 | [1..1] | Quantidade a ser dispensada por atendimento | Caracteres numéricos |  |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 8 | [1..1] | Unidade de medida do medicamento | Texto codificado | Unidade de medida do medicamento prescrito (ex.: comprimido, cápsula, frasco, caixa etc.) | [Unidade de Medida de Medicamento](ValueSet-BRUnidadeMedidaMedicamento.md) | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 7 | [0..1] | Duração de uso do medicamento | Caracteres alfanuméricos | Duração conforme ISO 8601 |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 7 | [0..1] | Total do tratamento | Caracteres numéricos | Quantidade total de medicamento prescrito. |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 7 | [0..1] | Orientações sobre o uso do medicamento | Texto livre |  |  | [Prescrição de Medicamento](StructureDefinition-BRPrescricaoMedicamento.md) |
| 4 | [1..1] | Status do uso do medicamento | Texto codificado: Ativo, Completado, Entrada com erro, Pretendido, Em pausa, Desconhecido, Não realizado | Informação sobre o uso da medicação por parte do paciente ou outro profissional (pode ser auto declarado ou referido). | [Estado da Solicitação de Medicamento](ValueSet-BREstadoSolicitacaoMedicamento-1.0.md) | [Medicamento](StructureDefinition-BRMedicamento.md) |

#### Plano de Cuidados, Instruções e Recomendações (Na Alta)

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [0..1] | Plano de cuidados, instruções e recomendações (na alta) |  |  |  |  |
| 2 | [1..1] | Descriçãodo plano de cuidados, instruções e recomendações | Texto livre |  |  | [Plano de Cuidados](StructureDefinition-BRPlanoCuidados-1.0.md) |

#### Dados do Desfecho

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [0..1] | Dados do desfecho |  |  |  |  |
| 2 | [0..1] | Desfecho | Texto codificado: Alta Clínica, Encaminhamento, Transferência, Retorno, Alta Voluntária, Ordem Judicial, Evasão, Óbito, Permanência, Sem registro no modelo de informação de origem | Caracteriza o motivo de conclusão do atendimento. | [Motivo do desfecho do Contato Assistencial](ValueSet-BRMotivoDesfecho-1.0.md) | [Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md) |
| 2 | [0..1] | Outras informações | Texto livre |  |  | [Outras Informações](StructureDefinition-BROutrasInformacoes.md), presente em[Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md) |

#### Atestado Médico/Odontológico

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [0..N] | Atestado Médico/Odontológico | Seção |  |  |  |
| 2 | [1..1] | Identificação do indivíduo |  | Identificador do indivíduo que recebe o Atestado |  | [Atestado Digital](StructureDefinition-BRAtestado.md) |
| 2 | [0..N] | Código da Classificação Internacional Doenças - Décima Revisão - CID-10 | Texto Codificado | Diagnóstico ou Problema que justifique o atestado |  | [CID10 Avaliado](StructureDefinition-BRCID10Avaliado-1.0.md) |
| 3 | [0..1] | Data do início do Diagnóstico/Problema | Texto codificado Iso 8601 | Data do inicio do problema ou Diagnóstico |  | [CID10 Avaliado](StructureDefinition-BRCID10Avaliado-1.0.md) |
| 2 | [1..1] | Data do inicio do Afastamento | Texto codificado Iso 8601 | Data de inicio do afastamento das atividades |  | [Atestado Digital](StructureDefinition-BRAtestado.md) |
| 2 | [1..1] | Tempo de afastamento (dias) | Caracteres numéricos | Número de dias que o paciente deve permanecer afastado das atividades |  | [Atestado Digital](StructureDefinition-BRAtestado.md) |
| 2 | [0..1] | Informações Adicionais | texto livre | Informações adicionais necessárias para documento atestado |  | [Atestado Digital](StructureDefinition-BRAtestado.md) |

#### Informações Adicionais/Complementares

| | | | | | | |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | [0..1] | Informações Adicionais/Complementares |  |  |  |  |
| 2 | [1..1] | Descrição das informações | Texto livre |  |  | [Contato Assistencial](StructureDefinition-BRContatoAssistencial-1.0.md) |

