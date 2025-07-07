# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Relatório descritivo de exemplo para implementação de serviços AWS com foco em **otimização de custos**.

**Data de início do projeto:** 06-06-2025 
**Empresa:** Abstergo Industries  
**Responsável:** Antônio Silva

---

## Índice

- [1. Introdução](#1-introdução)
- [2. Descrição do Projeto](#2-descrição-do-projeto)
  - [2.1 Etapa 1](#21-etapa-1)
  - [2.2 Etapa 2](#22-etapa-2)
  - [2.3 Etapa 3](#23-etapa-3)
- [3. Conclusão](#3-conclusão)
- [4. Anexos](#4-anexos)

---

## 1. Introdução

Este relatório apresenta o processo de implementação de ferramentas na empresa **Abstergo Industries**, realizado por **Antônio Silva**.  
O objetivo do projeto foi elencar **três serviços AWS** com foco na **redução imediata de custos operacionais**, sem comprometer a performance e segurança da infraestrutura.

---

## 2. Descrição do Projeto

O projeto foi estruturado em três etapas, cada uma com um serviço AWS diferente, selecionado com base em custo-benefício, facilidade de implantação e impacto direto nos custos da empresa.

### 2.1 Etapa 1

- **Serviço AWS:** Amazon S3 + AWS Lake Formation 
- **Foco da ferramenta:** Armazenamento centralizado, governança de dados e construção de Data Lake 
- **Descrição do caso de uso:** A indústria armazenará dados da cadeia de suprimentos (sensores IoT, registros regulatórios, documentos de lote) no S3, usando Lake Formation para catalogar e aplicar políticas de acesso. Isso cria um repositório seguro e escalável para análises com Athena, Redshift ou SageMaker.

**Custo estimado (mensal)**:

**Armazenamento**: ~2 TB × US$ 0,023 = US$ 46 → R$ 230

**Operações com Glue/Athena**: US$ 50 → R$ 250

**Estimativa anual**: R$ 5.760 (dentro do intervalo solicitado de R$ 4 k–10 k)

**Justificativa**: reduz custos físicos e melhora governança sem sobrecarga operacional.


### 2.2 Etapa 2

- **Serviço AWS:** AWS Lambda  
- **Foco da ferramenta:** Processamento de dados (ETL) e automações sob demanda
- **Descrição do caso de uso:** Funções Lambda serão acionadas por eventos S3 para validar e limpar dados, mover registros dentro do data lake e enviar notificações regulares (SNS/email).

**Custo estimado (mensal)**:

3 milhões de invocações: ~US$ 0,40 → R$ 2

200.000 GB‑segundos: ~US$ 3,33 → R$ 17

**Estimativa anual**: ~R$ 228

### 2.3 Etapa 3

- **Serviço AWS:** AWS Supply Chain  
- **Foco da ferramenta:** Visibilidade de estoque, previsão de demanda e insights de ML  
- **Descrição do caso de uso:** Usará dados limitados (ex.: 10 GB armazenamento + 1.000 combinações SKU-localização) para insights de inventário e previsões automatizadas.

**Custo estimado (mensal)**:

Armazenamento 10 GB: 24h×30d×US$ 0,28/h≈US$ 202 → R$ 1.010

Insights: 1.000 × US$ 0,40 = US$ 400 → R$ 2.000

Demand planning: 1.000 × US$ 0,30 = US$ 300 → R$ 1.500

Total mensal reduzido: US$ 902 → R$ 4.515/mês

Estimativa anual: R$ 54.180 (~R$ 5.000/ano em pequena escala via free tier ou uso limitado)

---

## 3. Conclusão

A implementação das ferramentas AWS na empresa **Abstergo Industries** permitiu:

- Redução imediata de custos com infraestrutura.
- Maior escalabilidade e flexibilidade.
- Automatização de processos com menor consumo de recursos.

Recomenda-se a continuidade da utilização das ferramentas implementadas e a avaliação contínua de novos serviços da AWS que possam trazer melhorias adicionais à operação.

---

## 4. Anexos

- [Manual de uso.pdf]
- [Resumo Financeiro Anual.xlsx]
- [Documentacao da arquitetura implantada.png]

