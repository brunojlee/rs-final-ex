# 🎯 Exercício Prático: Dashboard Material Design 3

> **Construa um dashboard moderno e profissional usando Material Design 3, MUI e Next.js com SEO otimizado**

![Material Design 3](https://img.shields.io/badge/Material%20Design-3-6750A4?style=for-the-badge&logo=material-design)
![Next.js](https://img.shields.io/badge/Next.js-14-000000?style=for-the-badge&logo=next.js)
![MUI](https://img.shields.io/badge/MUI-5-007FFF?style=for-the-badge&logo=mui)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript)

## 📋 Sobre o Exercício

Este exercício foi desenvolvido para **consolidar seus conhecimentos** em **Material Design 3**, **MUI v5**, **Next.js 14** e **SEO otimização**. Você irá construir um dashboard corporativo moderno seguindo as melhores práticas de desenvolvimento.

## 🎯 Objetivos de Aprendizado

Ao final deste exercício, você será capaz de:

✅ Implementar **Material Design 3** com fidelidade aos guidelines oficiais  
✅ Construir componentes **reutilizáveis** e **escaláveis** com MUI  
✅ Aplicar **Atomic Design** na arquitetura de componentes  
✅ Implementar **SEO otimizado** com Next.js 14  
✅ Gerenciar **temas** e **design tokens** profissionalmente  
✅ Criar interfaces **responsivas** e **acessíveis**  

## 🚀 Setup do Projeto

### 1. Instalação e Execução

```bash
# 1. Navegue até o diretório do projeto
cd aula3_project

# 2. Instale as dependências
npm install

# 3. Execute o servidor de desenvolvimento
npm run dev

# 4. Acesse no navegador
# http://localhost:3000
```

### 2. Estrutura do Projeto

```
src/
├── app/                     # App Router (Next.js 14)
│   ├── layout.tsx          # Layout principal
│   ├── page.tsx            # Página inicial (SEU EXERCÍCIO)
│   └── globals.css         # Estilos globais
├── components/             # Componentes reutilizáveis
│   ├── atoms/             # Componentes atômicos
│   ├── molecules/         # Componentes moleculares
│   ├── organisms/         # Componentes complexos
│   └── index.ts           # Exports centralizados
├── theme/                 # Sistema de design
│   ├── provider.tsx       # Provider do tema
│   ├── theme.ts          # Configuração do tema MUI
│   └── tokens.ts         # Design tokens MD3
└── types/                # Definições TypeScript
    └── index.ts
```

## 📝 Especificações do Exercício

### 🎨 **PARTE 1: Análise do Design System**

Antes de começar a codificar, analise os componentes já implementados:

1. **Explore a pasta `src/components/`**
   - Estude a estrutura Atomic Design
   - Analise como os design tokens são aplicados
   - Observe a integração com MUI

2. **Entenda o sistema de temas**
   - Arquivo: `src/theme/tokens.ts`
   - Como as cores Material Design 3 são implementadas
   - Sistema de espaçamento e tipografia

### 🏗️ **PARTE 2: Desenvolvimento da Interface**

#### **2.1 Header Component**
Implemente um header profissional que contenha:

```tsx
// Requisitos obrigatórios:
- Logo/título da aplicação
- Barra de pesquisa funcional
- Avatar do usuário
- Notificações (badge com contador)
- Toggle de tema (dark/light)
- Menu hambúrguer (mobile)
```

### 📱 **PARTE 3: Responsividade e Acessibilidade**

#### **3.1 Breakpoints**
Implemente comportamento responsivo para:
- **Mobile**: 320px - 768px
- **Tablet**: 768px - 1024px  
- **Desktop**: 1024px+


### 🔍 **PARTE 4: SEO Otimização**

#### **4.1 Metadata**
Configure no `src/app/layout.tsx`:

```tsx
export const metadata: Metadata = {
  title: 'Dashboard Corporativo | Sua Empresa',
  description: 'Dashboard executivo com métricas em tempo real, analytics avançados e relatórios corporativos.',
  keywords: 'dashboard, analytics, métricas, corporativo, business intelligence',
  authors: [{ name: 'Seu Nome' }],
  openGraph: {
    title: 'Dashboard Corporativo',
    description: 'Acompanhe métricas e KPIs em tempo real',
    type: 'website',
    locale: 'pt_BR'
  },
  twitter: {
    card: 'summary_large_image',
    title: 'Dashboard Corporativo',
    description: 'Métricas e analytics em tempo real'
  }
}
```

#### **4.2 Structured Data**
Adicione JSON-LD para melhor indexação:

```tsx
// Schema.org structured data
const jsonLd = {
  '@context': 'https://schema.org',
  '@type': 'WebApplication',
  'name': 'Dashboard Corporativo',
  'description': 'Plataforma de analytics e métricas corporativas',
  'url': 'https://seudominio.com'
}
```

## 🎨 Guidelines de Design

### **Cores (Material Design 3)**
```css
/* Principais */
--md-sys-color-primary: #6750A4
--md-sys-color-on-primary: #FFFFFF
--md-sys-color-secondary: #625B71
--md-sys-color-tertiary: #7D5260

/* Superfícies */
--md-sys-color-surface: #FEF7FF
--md-sys-color-surface-variant: #E7E0EC
```

### **Tipografia**
```css
/* Headlines */
Display Large: 57px/64px, Regular
Headline Large: 32px/40px, Regular  

/* Body */
Body Large: 16px/24px, Regular
Body Medium: 14px/20px, Regular
```

### **Espaçamento**
```css
/* Sistema baseado em 4px */
xs: 4px    sm: 8px     md: 16px
lg: 24px   xl: 32px    xxl: 48px
```

## ✅ Critérios de Avaliação

### **🔥 Obrigatórios (70 pontos)**
- [ ] Header funcional com todos os elementos
- [ ] Body funcional com todos os elementos
- [ ] Footer funcional com todos os elementos
- [ ] Design responsivo funcionando
- [ ] Design tokens aplicados corretamente
- [ ] SEO básico configurado

### **⭐ Diferenciais (30 pontos)**
- [ ] Animações e micro-interações
- [ ] Dark/Light theme funcional
- [ ] SEO otimizado (90+ Lighthouse)

## 🛠️ Comandos Úteis

```bash
# Desenvolvimento
npm run dev          # Servidor de desenvolvimento
npm run build        # Build de produção
npm run start        # Servidor de produção
npm run lint         # Verificar code quality
npm run type-check   # Verificar TypeScript

# Análise de bundle
npm install -g @next/bundle-analyzer
ANALYZE=true npm run build
```

## 📚 Recursos de Apoio

### **Documentação Oficial**
- [Material Design 3 Guidelines](https://m3.material.io/)
- [MUI Documentation](https://mui.com/material-ui/)
- [Next.js 14 Docs](https://nextjs.org/docs)

### **Ferramentas de Design**
- [Material Theme Builder](https://m3.material.io/theme-builder)
- [Material Design Icons](https://fonts.google.com/icons)
- [Color Tool](https://m3.material.io/styles/color/dynamic-color/overview)

### **SEO Tools**
- [Lighthouse](https://developers.google.com/web/tools/lighthouse)
- [Google Search Console](https://search.google.com/search-console)
- [Schema Markup Validator](https://validator.schema.org/)

## 🎯 Entrega

### **Formato de Entrega**
1. **Código fonte** completo e funcional
2. **README.md** com instruções de execução

## 💡 Dicas de Sucesso

### **🚀 Performance**
- Use `next/image` para otimização de imagens
- Implemente lazy loading nos componentes
- Minimize re-renders desnecessários
- Use `useMemo` e `useCallback` quando apropriado

### **🎨 Design**
- Mantenha consistência visual
- Use animações sutis (200-300ms)
- Respeite a hierarquia de informações
- Teste em diferentes dispositivos

### **📱 UX**
- Loading states em operações assíncronas
- Feedback visual para interações
- Estados de erro tratados
- Navegação intuitiva

## 🏆 Boa Sorte!

Este exercício é uma oportunidade de aplicar conhecimentos avançados em desenvolvimento front-end moderno. Foque na qualidade do código, atenção aos detalhes e experiência do usuário.

**Lembre-se**: O objetivo é aprender e evoluir. Não hesite em experimentar e iterar suas soluções!

