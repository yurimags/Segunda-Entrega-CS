# Estrutura Modular de CSS - Segunda Entrega CS

## 📁 Organização de Arquivos

```
css/
├── base/
│   ├── _reset.css          # Reset CSS e normalização
│   ├── _variables.css       # Sistema de design (cores, tipografia, espaçamentos)
│   └── _typography.css      # Estilos tipográficos hierárquicos
├── layout/
│   ├── _grid-system.css     # Sistema de grid customizado (12 colunas)
│   ├── _layout.css          # Leiautes principais com CSS Grid
│   └── _responsive.css      # Breakpoints responsivos (5+ breakpoints)
├── components/
│   ├── _navigation.css      # Navegação com dropdown e hambúrguer
│   ├── _buttons.css         # Botões com estados (hover, focus, active, disabled)
│   ├── _cards.css            # Cards responsivos
│   ├── _forms.css            # Formulários estilizados com validação visual
│   ├── _badges-tags.css      # Sistema de badges e tags
│   ├── _alerts.css           # Componentes de alerta
│   ├── _toasts.css           # Notificações temporárias (toasts)
│   └── _modals.css           # Janelas modais
├── utilities/
│   └── _utilities.css        # Classes utilitárias (margins, padding, display, etc.)
└── styles.css                # Arquivo principal que importa todos os módulos
```

## ✅ Especificações Implementadas

### 1. Sistema de Design
- ✅ Variáveis CSS customizadas em `_variables.css`
- ✅ Paleta de cores com 8+ cores (primárias, secundárias, neutras, feedback)
- ✅ Tipografia hierárquica com 5+ tamanhos de fonte
- ✅ Sistema de espaçamento modular (8px, 16px, 24px, 32px, 48px, 64px)

### 2. Leiautes Responsivos
- ✅ CSS Grid para estrutura geral (`_layout.css`)
- ✅ Flexbox para componentes internos
- ✅ 5+ breakpoints bem definidos:
  - Mobile Extra Small: 320px+
  - Mobile Small: 576px+
  - Tablet: 768px+
  - Desktop: 992px+
  - Desktop Large: 1200px+
  - Desktop Extra Large: 1400px+
- ✅ Sistema de grid customizado de 12 colunas (`_grid-system.css`)
- ✅ Leiautes específicos para diferentes tipos de conteúdo

### 3. Navegação Sofisticada
- ✅ Menu principal com submenu dropdown
- ✅ Menu hambúrguer para mobile
- ✅ Overlay para mobile
- ✅ Controle via JavaScript para abertura/fechamento
- ✅ Acessibilidade (aria-expanded, tecla ESC)

### 4. Componentes de Interface
- ✅ Cards responsivos para projetos (`_cards.css`)
- ✅ Botões com estados visuais completos:
  - hover
  - focus
  - active
  - disabled
- ✅ Formulários estilizados com validação visual (`_forms.css`)
- ✅ Componentes de feedback:
  - Alerts (`_alerts.css`)
  - Toasts (`_toasts.css`)
  - Modals (`_modals.css`)
- ✅ Sistema de badges e tags (`_badges-tags.css`)

## 🎨 Paleta de Cores

### Cores Primárias
- `--color-primary`: #2c5aa0
- `--color-primary-dark`: #1e3f70
- `--color-primary-light`: #4a90e2

### Cores Secundárias
- `--color-secondary`: #4a90e2
- `--color-secondary-dark`: #357abd

### Cores de Acentuação
- `--color-accent`: #28a745
- `--color-accent-dark`: #218838

### Cores Neutras (10 tons)
- De `--color-neutral-900` a `--color-neutral-50`

### Cores de Feedback
- Success: #28a745
- Error: #dc3545
- Warning: #ffc107
- Info: #17a2b8

## 📐 Sistema de Espaçamento

Espaçamentos modulares baseados em 8px:
- `--spacing-xs`: 4px (0.25rem)
- `--spacing-sm`: 8px (0.5rem)
- `--spacing-md`: 16px (1rem)
- `--spacing-lg`: 24px (1.5rem)
- `--spacing-xl`: 32px (2rem)
- `--spacing-2xl`: 48px (3rem)
- `--spacing-3xl`: 64px (4rem)

## 📝 Tipografia

Tamanhos hierárquicos:
- `--font-size-xs`: 12px
- `--font-size-sm`: 14px
- `--font-size-base`: 16px
- `--font-size-md`: 18px
- `--font-size-lg`: 20px
- `--font-size-xl`: 24px
- `--font-size-2xl`: 32px
- `--font-size-3xl`: 40px
- `--font-size-4xl`: 48px

## 🎯 Breakpoints Responsivos

| Breakpoint | Largura | Uso |
|------------|---------|-----|
| XS | 320px+ | Mobile extra small |
| SM | 576px+ | Mobile small |
| MD | 768px+ | Tablet |
| LG | 992px+ | Desktop |
| XL | 1200px+ | Desktop large |
| 2XL | 1400px+ | Desktop extra large |

## 🔧 Como Usar

### Importar CSS
O arquivo `styles.css` já importa todos os módulos. Basta incluir no HTML:
```html
<link rel="stylesheet" href="css/styles.css">
```

### Usar Classes do Grid
```html
<div class="container">
  <div class="row">
    <div class="col-md-6 col-lg-4">Conteúdo</div>
    <div class="col-md-6 col-lg-8">Conteúdo</div>
  </div>
</div>
```

### Usar Componentes
```html
<!-- Botão -->
<a href="#" class="btn btn-primary">Clique aqui</a>

<!-- Card -->
<div class="card">Conteúdo do card</div>

<!-- Badge -->
<span class="badge badge-success">Novo</span>

<!-- Alert -->
<div class="alert alert-success">
  <strong>Sucesso!</strong> Operação realizada.
</div>
```

## 📱 Navegação Mobile

A navegação inclui:
- Menu hambúrguer animado
- Menu lateral deslizante
- Overlay escuro ao abrir
- Fechamento automático ao clicar em link
- Suporte a tecla ESC para fechar

## ✨ Recursos Adicionais

- Animações suaves em transições
- Sombras hierárquicas (sm, md, lg, xl)
- Border radius consistente
- Sistema de z-index organizado
- Classes utilitárias para espaçamento
- Suporte completo a acessibilidade

## 🚀 Próximos Passos (Opcional)

Para expandir o sistema:
- Adicionar tema escuro (dark mode)
- Criar mais componentes específicos
- Implementar animações mais complexas
- Adicionar documentação de Storybook

