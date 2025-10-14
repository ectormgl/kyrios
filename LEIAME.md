# KYRIOS - Site de Serviços de IA

Bem-vindo ao site da Kyrios! Este é um site estático moderno e responsivo, construído com HTML e CSS puros.

## 🎨 Visão Geral do Design

- **Esquema de Cores**: Preto (#0a0a0a), Amarelo (#FFF82C), Ciano (#00E5FF)
- **Tipografia**: Android (títulos), Roboto (corpo do texto)
- **Estilo**: Moderno, minimalista, profissional

## 📁 Estrutura do Projeto

```
website/
├── index.html          # Página principal
├── blog.html           # Página de Blog/Notícias
├── css/
│   ├── style.css       # Folha de estilos principal
│   └── blog.css        # Estilos específicos do blog
├── js/
│   └── script.js       # Funcionalidades JavaScript
└── assets/
    └── images/         # Todas as imagens e logos
```

## 🚀 Funcionalidades

### Página Principal (index.html)
- **Seção Hero**: Landing atraente com logo animado
- **Seção Sobre**: Visão geral da empresa com estatísticas animadas
- **Seção Serviços**: Dois serviços em destaque (Desenvolvimento de Agentes de IA e Consultoria)
- **Seção Portfólio**: Showcase de 3 projetos de clientes
- **Seção Equipe**: Perfis dos membros da equipe
- **Seção Contato**: Informações de contato e integração com WhatsApp

### Página de Blog (blog.html)
- **Posts do Blog**: Layout em grid com posts em destaque e regulares
- **Barra Lateral**: Busca, categorias, posts recentes, inscrição newsletter, tags
- **Paginação**: Navegação entre posts do blog

### Recursos Interativos
- Navegação com rolagem suave
- Menu responsivo para mobile
- Elementos animados no scroll
- Botão flutuante do WhatsApp
- Destaque ativo da navegação

## 📱 Integração com WhatsApp

O site inclui funcionalidade de contato via WhatsApp:
- Botão flutuante do WhatsApp (canto inferior direito)
- Botão na seção de contato
- **IMPORTANTE**: Atualize o número de telefone nestes arquivos:
  - `index.html` (procure por `15551234567` e substitua)
  - `blog.html` (procure por `15551234567` e substitua)

Formato: `https://wa.me/NUMERODETELEFONE` (incluir código do país, sem + ou espaços)
Exemplo: `https://wa.me/5511999998888` para Brasil

## ✏️ Guia de Personalização

### 1. Atualizar Informações de Contato

**No `index.html`, encontre e atualize:**

```html
<!-- E-mail -->
<p>contact@kyrios.ai</p>

<!-- Telefone -->
<p>+1 (555) 123-4567</p>

<!-- Localização -->
<p>São Paulo, SP</p>

<!-- WhatsApp -->
href="https://wa.me/15551234567..."
```

### 2. Adicione Suas Imagens

Substitua as imagens placeholder em `assets/images/`:

**Imagens Necessárias:**
- `logo-symbol.svg` - Já incluído (seu logo)
- `client-1.jpg` - Imagem do portfólio 1 (recomendado: 800x500px)
- `client-2.jpg` - Imagem do portfólio 2 (recomendado: 800x500px)
- `client-3.jpg` - Imagem do portfólio 3 (recomendado: 800x500px)
- `team-1.jpg` - Foto do membro da equipe (recomendado: 400x400px)
- `team-2.jpg` - Foto do membro da equipe (recomendado: 400x400px)
- `team-3.jpg` - Foto do membro da equipe (recomendado: 400x400px)

**Imagens do Blog (opcional):**
- `blog-featured.jpg` - Post em destaque (1200x600px)
- `blog-1.jpg` a `blog-5.jpg` - Posts do blog (800x400px)
- `blog-thumb-1.jpg` a `blog-thumb-3.jpg` - Miniaturas (150x150px)

### 3. Atualizar Informações da Equipe

No `index.html`, encontre a Seção da Equipe e atualize:

```html
<h4 class="member-name">Seu Nome</h4>
<p class="member-role">Seu Cargo</p>
```

### 4. Modificar Serviços

Para adicionar ou modificar serviços, edite a Seção de Serviços em `index.html`. Cada serviço usa esta estrutura:

```html
<div class="service-card featured">
    <div class="service-icon">
        <!-- Ícone SVG aqui -->
    </div>
    <h3 class="service-title">Nome do Serviço</h3>
    <p class="service-description">Descrição...</p>
    <ul class="service-features">
        <li>Recurso 1</li>
        <li>Recurso 2</li>
    </ul>
</div>
```

### 5. Atualizar Posts do Blog

No `blog.html`, cada post do blog segue esta estrutura:

```html
<article class="blog-post">
    <div class="post-image">
        <img src="assets/images/blog-1.jpg" alt="Post do Blog">
    </div>
    <div class="post-content">
        <div class="post-meta">
            <span class="post-category">Categoria</span>
            <span class="post-date">Data</span>
        </div>
        <h3 class="post-title">Título do Post</h3>
        <p class="post-excerpt">Resumo do post...</p>
        <a href="#" class="post-link">Leia Mais →</a>
    </div>
</article>
```

### 6. Atualizar Links de Redes Sociais

Encontre e substitua `#` com seus URLs reais de redes sociais:

```html
<!-- LinkedIn -->
<a href="SUA_URL_DO_LINKEDIN" aria-label="LinkedIn">

<!-- Twitter -->
<a href="SUA_URL_DO_TWITTER" aria-label="Twitter">

<!-- Instagram -->
<a href="SUA_URL_DO_INSTAGRAM" aria-label="Instagram">
```

## 🌐 Deploy no GitHub Pages

1. **Crie um novo repositório** no GitHub
2. **Envie a pasta do site** para o repositório
3. **Habilite o GitHub Pages**:
   - Vá para Settings do repositório
   - Role até a seção "Pages"
   - Selecione o branch "main" como source
   - Selecione a pasta "/ (root)"
   - Clique em Save
4. Seu site estará ao vivo em: `https://seuusuario.github.io/nome-do-repositorio/`

### Importante para o GitHub Pages:
- Certifique-se que `index.html` está no diretório raiz
- Todos os caminhos de arquivos devem ser relativos (já configurado)
- As imagens devem estar na pasta `assets/images/`

## 🔧 Suporte de Navegadores

- Chrome (mais recente)
- Firefox (mais recente)
- Safari (mais recente)
- Edge (mais recente)
- Navegadores móveis (iOS Safari, Chrome Mobile)

## 📝 Observações

- O site é totalmente responsivo e compatível com dispositivos móveis
- Todas as animações são otimizadas para performance
- O design segue suas diretrizes de marca (amarelo #FFF82C e ciano #00E5FF)
- Não requer dependências externas (exceto Google Fonts)
- Site estático - não requer backend

## 🎯 Melhorias Futuras (Opcional)

Se você quiser adicionar mais recursos posteriormente:
- Formulário de contato com integração de backend
- Integração CMS para blog
- Widget de chat ao vivo
- Rastreamento de analytics (Google Analytics)
- Otimização de SEO
- Otimização de performance

## 📞 Suporte

Para dúvidas sobre o site:
- Revise os comentários no código dos arquivos HTML/CSS
- Todas as seções estão claramente rotuladas
- Verifique o console para erros (F12 no navegador)

---

**Construído com ❤️ para Kyrios Serviços de IA**

Última Atualização: 14 de Outubro, 2025
