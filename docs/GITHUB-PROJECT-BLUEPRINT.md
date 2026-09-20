# GitHub Project — Blueprint do Case 06

Este documento define a reconstrução executiva e anonimizada do case **Facilities: Desmobilização e Consolidação Operacional**.

O case consolida duas iniciativas reais e relacionadas, sem transformá-las artificialmente em um único projeto:
- **Workplace Consolidation** — desmobilização de escritórios, realocação, regularizações e Flexoffice;
- **Facility Decommissioning** — desmobilização de unidade logística, ativos, infraestrutura, fornecedores, obras e encerramento.

## Fonte dos cards

Foram definidos 14 cards históricos representativos, reconstruídos a partir da lógica real de governança e execução.

## Campos recomendados no GitHub Project

| Campo | Tipo | Valores sugeridos |
|---|---|---|
| Status | Single select | Concluído |
| Iniciativa | Single select | Workplace Consolidation; Facility Decommissioning |
| Workstream | Single select | Governança; Workplace; Legal; Facilities; Ativos; Tecnologia; Fornecedores; Financeiro; Encerramento |
| Tipo | Single select | Governança; Entrega; Dependência; Risco; Decisão; Change Request; Encerramento |
| Risco histórico | Single select | Baixo; Médio; Alto |
| Dependência externa | Single select | Sim; Não |
| Marco | Single select | Estruturação; Transição; Desmobilização; Vistoria; Regularização; Encerramento |

## Views recomendadas

### 1. Executive Overview
**Layout:** Table  
**Group by:** Iniciativa  
**Sort:** Marco

Campos visíveis:
- Title
- Iniciativa
- Workstream
- Marco
- Risco histórico
- Dependência externa
- Status

### 2. Workplace Consolidation
**Layout:** Board  
**Filtro:** Iniciativa = Workplace Consolidation  
**Group by:** Workstream

### 3. Facility Decommissioning
**Layout:** Board  
**Filtro:** Iniciativa = Facility Decommissioning  
**Group by:** Workstream

### 4. Riscos & Dependências
**Layout:** Table  
**Filtro:** Risco histórico = Alto OR Dependência externa = Sim

### 5. Encerramento
**Layout:** Table  
**Filtro:** Workstream = Encerramento OR Tipo = Change Request

## Cards de destaque

- **Preparar continuidade operacional antes da saída do escritório**
- **Inventariar e destinar ativos antes da movimentação**
- **Formalizar Change Request após vistoria final**
- **Registrar pendência contratual residual no encerramento**

## Regra de confidencialidade

Não adicionar ao Project:
- nomes reais dos imóveis;
- endereços;
- nomes de colaboradores;
- fornecedores;
- contratos;
- valores;
- identificadores internos;
- documentos originais;
- dados cadastrais ou societários;
- detalhes técnicos que identifiquem a infraestrutura real.

## Resultado esperado

O GitHub Project deve funcionar como um **digital twin executivo e anonimizado** das duas iniciativas, demonstrando a lógica de governança sem reproduzir o ambiente corporativo.
