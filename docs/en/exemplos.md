# Exemplos - Guia de Implementação do Registro de Atendimento Clínico (RAC) da RNDS v1.0.0-release

## Exemplos

### Exemplos

 [Exemplo de Bundle do Registro de Atendimento Clínico (RAC) - Paciente Identificado](Bundle-bundle-example-rac-1.md) 

#### Caso de uso para Paciente Identificado

 Em uma tarde de 9 de maio de 2022, por volta das 15:36, um paciente (identificado na API como 819217217061851) chegou a uma unidade de saúde queixando-se da presença de sangue na saliva. O paciente foi prontamente atendido em caráter ambulatorial (modalidade assistencial 04). 

```
{
      "subject": {
        "identifier": {
          "system": "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuo-1.0",
          "value": "819217217061851"
        }
      }
    }
```

```
{
        "hospitalization": {
          "extension": [
            {
              "url": "http://www.saude.gov.br/fhir/r4/StructureDefinition/BROutrasInformacoes",
              "valueAnnotation": {
                "text": "Paciente se queixando da presença de sangue na saliva.",
                "time": "2022-05-09"
              }
            }
          ]
        },
        "period": {
          "start": "2022-04-09T15:36:40.157-03:00",
          "end": "2022-05-09T15:46:48.534-03:00"
        }
      }
```

 Durante a avaliação inicial, foram coletadas diversas medidas do paciente: 

* Altura: 1,83 metros
* Perímetro cefálico: 135,5 cm
* Peso: 88,15 kg (pesado com roupas leves)
* Pressão arterial: 0,15 mmHg (medida no braço direito)

```
{
      "resourceType": "Observation",
      "code": {
        "coding": [
          {
            "system": "http://loinc.org",
            "code": "8302-2"
          }
        ]
      },
      "valueQuantity": {
        "value": 1.83,
        "system": "http://unitsofmeasure.org",
        "code": "m"
      }
    }
```

```
{
        "resourceType": "Observation",
        "code": {
          "coding": [
            {
              "system": "http://loinc.org",
              "code": "29463-7"
            }
          ]
        },
        "valueQuantity": {
          "value": 88.15,
          "system": "http://unitsofmeasure.org",
          "code": "kg"
        }
      }
```

 Na anamnese, o profissional identificou que o paciente fazia uso ocasional de álcool ("uma ou duas vezes") e cannabis. 

```
{
      "resourceType": "Observation",
      "code": {
        "coding": [
          {
            "system": "http://loinc.org",
            "code": "56832-9"
          }
        ]
      },
      "effectiveTiming": {
        "code": {
          "coding": [
            {
              "system": "http://www.saude.gov.br/fhir/r4/CodeSystem/BRFrequenciaUsoSubstancia",
              "code": "uma-ou-duas"
            }
          ]
        }
      },
      "valueCodeableConcept": {
        "coding": [
          {
            "system": "http://www.saude.gov.br/fhir/r4/CodeSystem/BRTipoSubstanciaUso",
            "code": "alcool"
          }
        ]
      },
      "note": [
        {
          "text": "Uso ocasional de cannabis."
        }
      ]
    }
```

 Após avaliação, o médico diagnosticou o paciente com varizes esofagianas sem sangramento (CID I859). Foi realizada uma consulta médica (código do procedimento: 0301010048) e prescrito um medicamento via oral, que deveria ser tomado uma vez ao dia, com dosagem de 10 unidades por administração. 

```
{
      "resourceType": "Condition",
      "code": {
        "coding": [
          {
            "system": "http://www.saude.gov.br/fhir/r4/CodeSystem/BRCID10",
            "code": "I859"
          }
        ]
      },
      "note": [
        {
          "text": "Varizes esofagianas sem sangramento."
        }
      ]
    }
```

 O médico responsável, Dr. Getúlio, deixou instruções específicas para o uso do medicamento, indicando que era necessário para tratamento da febre devido à gripe. A prescrição foi válida por uma semana, de 24 de fevereiro a 3 de março de 2022. 

```
{
      "resourceType": "MedicationRequest",
      "note": [
        {
          "authorString": "Dr. Getúlio",
          "time": "2022-03-04",
          "text": "Medicamento necessário para tratamento da febre devido à gripe."
        }
      ],
      "dosageInstruction": [
        {
          "patientInstruction": "Tomar uma vez ao dia via oral.",
          "timing": {
            "repeat": {
              "count": 1,
              "countMax": 10,
              "frequency": 12
            }
          }
        }
      ],
      "dispenseRequest": {
        "validityPeriod": {
          "start": "2022-02-24",
          "end": "2022-03-03"
        },
        "quantity": {
          "value": 10
        }
      }
    }
```

 Durante o atendimento, também foi identificada uma alergia ao soro antitetânico (SAT), classificada como de baixa criticidade, com reações documentadas. 

```
{
      "resourceType": "AllergyIntolerance",
      "criticality": "low",
      "code": {
        "coding": [
          {
            "system": "http://www.saude.gov.br/fhir/r4/CodeSystem/BRImunobiologico",
            "code": "2"
          }
        ],
        "text": "SAT"
      },
      "note": [
        {
          "text": "Soro antitetânico"
        }
      ]
    }
```

 O paciente recebeu orientações para repouso pós-medicação intramuscular como parte de seu plano de cuidados. O atendimento foi finalizado por volta das 15:46, com encaminhamento do paciente (código de desfecho 06). 

```
{
      "resourceType": "CarePlan",
      "status": "active",
      "intent": "plan",
      "description": "Repouso pós-medicação intramuscular"
    }
```

 [Exemplo de Bundle do Registro de Atendimento Clínico (RAC) - Paciente Não Identificado](Bundle-bundle-example-rac-2.md) 

#### Caso de uso para Paciente Não Identificado

 Em essência, as informações, como medidas sintomas e diagnósticos são as mesmas do exemplo do paciente identificado. As principais diferenças são a ausência do horário do atendimento e a coleta de dados que não facilitem sua identificação, sendo considerado apenas um jovem homem de aproximadamente 22 anos (nascido em 2000). Na estrutura da API ele pode ser encontrado como: 

```
{
    "subject": {
      "extension": [
        {
          "url": "http://www.saude.gov.br/fhir/r4/StructureDefinition/BRIndividuoNaoIdentificado-1.0",
          "extension": [
            {
              "url": "gender",
              "valueCode": "male"
            },
            {
              "url": "birthYear",
              "valueDate": "2000"
            },
            {
              "url": "reason",
              "valueCodeableConcept": {
                "coding": [
                  {
                    "system": "http://www.saude.gov.br/fhir/r4/CodeSystem/BRJustificativaIndividuoNaoIdentificado",
                    "code": "01"
                  }
                ]
              }
            }
          ]
        }
      ]
    }
  }
```

