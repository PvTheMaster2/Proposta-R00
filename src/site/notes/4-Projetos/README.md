---
{"dg-publish":true,"permalink":"/4-projetos/readme/","title":"Portfólio de Projetos","noteIcon":""}
---

# 📋 GESTÃO DE PROJETOS

> *Iniciativas e projetos da empresa*

---

## 🎯 **PROPÓSITO**

Esta pasta contém todos os projetos e iniciativas da empresa, organizados por status e tipo. Utiliza frontmatter padronizado para facilitar consultas Dataview e automação.

---

## 📁 **ESTRUTURA DE SUBPASTAS**

### **Ativos/**
- **Propósito**: Projetos em andamento
- **Status**: Projetos com status "in-progress"
- **Conteúdo**: Projetos ativos sendo executados

### **Concluidos/**
- **Propósito**: Projetos finalizados
- **Status**: Projetos com status "deployed" ou "archived"
- **Conteúdo**: Projetos concluídos com sucesso

### **Backlog/**
- **Propósito**: Ideias aprovadas
- **Status**: Projetos com status "idea" ou "planning"
- **Conteúdo**: Ideias aprovadas aguardando execução

### **Pilotos/**
- **Propósito**: Experimentos e pilotos
- **Subpastas**:
  - **Ideias/** - Ideias de pilotos
  - **Em-Execucao/** - Pilotos ativos

---

## 📊 **FRONTMATTER PADRONIZADO**

### **Campos Obrigatórios**
```yaml
---
template: projeto-empresarial
type: project                    # project | pilot
status: idea                     # idea | planning | in-progress | pilot | deployed | archived
priority: medium                 # low | medium | high | critical
owner: ""                       # formato [[Nome]]
market_segment: ""              # segmento de mercado
effort_weeks: 0                 # inteiro (esforço em semanas)
budget: 0                       # numérico R$ (sem formatação)
metrics_first_month: ""         # string comparável
ia_assets:                      # assets de IA utilizados
  prompts: []                   # lista de prompts
  models: []                    # modelos utilizados
  datasets: []                  # datasets necessários
compliance_level: 1             # 1=básico | 2=dados | 3=crítico
legal_review: false             # boolean
created: {{date}}               # timestamp criação
modified: {{date}}              # timestamp modificação
---
```

---

## 📈 **QUERIES DATAVIEW ÚTEIS**

### **Todos os Projetos**
| File | Status | Projeto | Owner | Esforço | Budget |
| ---- | ------ | ------- | ----- | ------- | ------ |

{ .block-language-dataview}

### **Projetos por Status**
| status | Quantidade | Orçamento Total (R$) |
| ------ | ---------- | -------------------- |

{ .block-language-dataview}

### **Projetos por Prioridade**
| priority | Quantidade | Orçamento Total (R$) |
| -------- | ---------- | -------------------- |

{ .block-language-dataview}

---

## 🔗 **LINKS RÁPIDOS**

- [[0-Dashboard-Executivo/Innovation-Pipeline\|0-Dashboard-Executivo/Innovation-Pipeline]] - Dashboard de pipeline
- [[z_Templates/Projetos/\|z_Templates/Projetos/]] - Templates de projetos
- [[5-Processos/README\|5-Processos/README]] - Processos de gestão
- [[6-Reunioes/README\|6-Reunioes/README]] - Reuniões de projetos

---

## 📋 **TEMPLATES DISPONÍVEIS**

- **project.md** - Template para projetos principais
- **pilot.md** - Template para pilotos e experimentos
- **task.md** - Template para tarefas
- **sprint.md** - Template para sprints
- **person.md** - Template para pessoas

---

**Status**: 🔄 **EM DESENVOLVIMENTO**  
**Próximo**: Implementar templates e automação
