# 💜 Convite Digital - Chá de Fralda da Luiza

> Um convite digital elegante e responsivo para chá de fraldas, com design em tons de lavanda e sistema integrado de confirmação de presença.

---

## 📋 Sumário

- [Visão Geral](#-visão-geral)
- [Características](#-características)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Como Usar](#-como-usar)
- [Configuração e Personalização](#-configuração-e-personalização)
- [Integração com Serviços Externos](#-integração-com-serviços-externos)
- [Design e Estilo](#-design-e-estilo)
- [Responsividade](#-responsividade)
- [Otimizações](#-otimizações)

---

## 🎯 Visão Geral

Este projeto consiste em um **convite digital interativo** para o Chá de Fralda da Luiza, desenvolvido com HTML5 e CSS3 puro, sem dependência de frameworks JavaScript. O convite inclui:

- **Página principal** (`index.html`) com todas as informações do evento
- **Página de RSVP** (`rsvp.html`) para confirmação de presença
- **Integração** com Google Forms e Google Maps
- **Design responsivo** otimizado para compartilhamento via WhatsApp

### 📅 Detalhes do Evento

- **Data:** 13 de Junho de 2026
- **Horário:** 13h
- **Local:** Chácara da Vovó Lu, São Sebastião - Paracatu/MG
- **Tema:** Feijoada e Chá de Fralda

---

## ✨ Características

### Página Principal (index.html)

- ✅ Design elegante com paleta de cores lavanda
- ✅ Animações suaves de elementos decorativos (corações flutuantes)
- ✅ Informações completas do evento (data, hora, local)
- ✅ Botão de navegação para Google Maps
- ✅ Botão de confirmação de presença integrado
- ✅ Meta tags Open Graph para preview bonito no WhatsApp
- ✅ Ícones SVG inline para melhor performance
- ✅ Design totalmente responsivo

### Página de RSVP (rsvp.html)

- ✅ Formulário completo de confirmação de presença
- ✅ Campos de entrada:
  - Nome completo
  - Telefone/WhatsApp
  - Confirmação (Sim/Não) com botões estilizados
  - Número de acompanhantes (stepper interativo)
  - Seleção de tamanho de fralda (P/M/G/XG)
  - Observações adicionais (textarea)
- ✅ Validação HTML5 nativa
- ✅ Integração com Google Forms via iframe
- ✅ Design consistente com a página principal
- ✅ Feedback visual para interações do usuário

---

## 🛠 Tecnologias Utilizadas

### Frontend

| Tecnologia | Versão | Uso |
|-----------|--------|-----|
| **HTML5** | - | Estrutura semântica das páginas |
| **CSS3** | - | Estilização e animações |
| **JavaScript (Vanilla)** | ES6+ | Interatividade do formulário RSVP |

### Fontes

- **Cormorant Garamond** (Serif) - Títulos e datas
- **Great Vibes** (Cursiva) - Nome "Luiza"
- **Montserrat** (Sans-serif) - Texto geral

### Integrações Externas

- **Google Forms** - Sistema de coleta de confirmações
- **Google Maps** - Localização do evento
- **Google Fonts** - Tipografias customizadas

---

## 📁 Estrutura do Projeto

```
convite-cha-fralda-luiza/
│
├── index.html                          # Página principal do convite
├── rsvp.html                           # Página de confirmação de presença
├── README.md                           # Documentação do projeto
│
├── Link formulario presença.txt        # URL do Google Forms
├── Link mapa da localização.txt        # URL do Google Maps
└── Sugestão de texto.txt               # Texto de referência para o convite
```

---

## 🚀 Como Usar

### 1. Hospedagem

O projeto pode ser hospedado em qualquer serviço de hospedagem estática:

#### Opções Recomendadas (Gratuitas):

- **GitHub Pages**
  ```bash
  # 1. Crie um repositório no GitHub
  # 2. Faça upload dos arquivos index.html e rsvp.html
  # 3. Ative GitHub Pages nas configurações do repositório
  # 4. Acesse via: https://seu-usuario.github.io/nome-repositorio
  ```

- **Netlify**
  ```bash
  # 1. Arraste a pasta do projeto para netlify.com/drop
  # 2. URL será gerada automaticamente
  ```

- **Vercel**
  ```bash
  # 1. Importe o repositório em vercel.com
  # 2. Deploy automático
  ```

### 2. Compartilhamento

Após hospedar, compartilhe o link via:

- **WhatsApp** (preview otimizado com Open Graph)
- **Email**
- **Redes Sociais**

### 3. Teste Local

Para testar localmente:

```bash
# Método 1: Abrir diretamente no navegador
# - Clique duas vezes em index.html

# Método 2: Servidor HTTP simples (recomendado)
# Python 3.x:
python -m http.server 8000

# Node.js (com npx):
npx serve .

# Acesse: http://localhost:8000
```

---

## ⚙ Configuração e Personalização

### Modificar Informações do Evento

#### No arquivo `index.html`:

1. **Nome do bebê** (linha 108):
```html
<div class="name">Luiza</div>
```

2. **Data e horário** (linhas 116-118):
```html
<div class="date">13 de Junho</div>
<div class="time">13h</div>
```

3. **Local** (linhas 119-121):
```html
<div class="place">
  Chácara da Vovó Lu
  <small>São Sebastião · Paracatu, MG</small>
</div>
```

4. **Link do Google Maps** (linha 127):
```html
<a href="https://maps.app.goo.gl/5Ax6LFdp67cN6rSF9" ...>
```

### Alterar Cores do Tema

#### No arquivo CSS (linhas 20-28 em ambos os arquivos):

```css
:root {
  --lavender-deep: #6b4a8b;      /* Lavanda escuro */
  --lavender: #8a6fb0;            /* Lavanda principal */
  --lavender-soft: #b89dd4;       /* Lavanda suave */
  --lavender-bg: #f5f0fa;         /* Fundo lavanda claro */
  --lavender-bg-2: #ece3f5;       /* Fundo lavanda médio */
  --cream: #fbf8fc;               /* Creme */
  --text: #4a3a5e;                /* Texto principal */
  --gold: #c9a96e;                /* Dourado (decorativo) */
}
```

### Personalizar o Formulário RSVP

#### No arquivo `rsvp.html`:

1. **URL do Google Forms** (linha 241):
```html
<iframe src="https://forms.gle/evssPvXSW4XRGp189" ...>
```

2. **Opções de tamanho de fralda** (linhas 197-200):
```html
<option value="P">P (até 5 kg)</option>
<option value="M" selected>M (5-9 kg)</option>
<option value="G">G (9-12 kg)</option>
<option value="XG">XG (12+ kg)</option>
```

---

## 🔗 Integração com Serviços Externos

### Google Forms

O formulário RSVP utiliza um Google Forms embutido via iframe para coletar confirmações de presença.

**Configuração:**

1. Crie um novo Google Forms
2. Configure os campos necessários:
   - Nome
   - Telefone
   - Confirmação de presença
   - Número de acompanhantes
   - Tamanho da fralda
   - Observações
3. Obtenha o link de compartilhamento
4. Substitua a URL no arquivo `rsvp.html` (linha 241)

**URL atual:**
```
https://forms.gle/evssPvXSW4XRGp189
```

### Google Maps

O botão "Ver no Mapa" leva diretamente ao local do evento no Google Maps.

**Configuração:**

1. Acesse [Google Maps](https://maps.google.com)
2. Busque o endereço: "Chácara da Vovó Lu, São Sebastião, Paracatu - MG"
3. Clique em "Compartilhar" → "Copiar link"
4. Substitua a URL no arquivo `index.html` (linha 127)

**URL atual:**
```
https://maps.app.goo.gl/5Ax6LFdp67cN6rSF9
```

**Coordenadas:** Q5W7+R6 - São Sebastião, Paracatu - MG, 38600-000

---

## 🎨 Design e Estilo

### Paleta de Cores

| Cor | Hex Code | Uso |
|-----|----------|-----|
| Lavanda Profundo | `#6b4a8b` | Títulos, texto de destaque |
| Lavanda Principal | `#8a6fb0` | Nome, destaques, bordas ativas |
| Lavanda Suave | `#b89dd4` | Elementos decorativos, hover |
| Fundo Lavanda | `#f5f0fa` | Backgrounds secundários |
| Creme | `#fbf8fc` | Background do card |
| Texto | `#4a3a5e` | Texto principal |
| Dourado | `#c9a96e` | Elementos decorativos |

### Tipografia

```css
/* Títulos e Datas */
font-family: 'Cormorant Garamond', serif;
font-weight: 500-600;

/* Nome "Luiza" */
font-family: 'Great Vibes', cursive;
font-size: 92px (desktop) / 72px (mobile);

/* Corpo do Texto */
font-family: 'Montserrat', sans-serif;
font-weight: 300-600;
```

### Animações

#### Corações Flutuantes
```css
@keyframes float {
  0%, 100% { transform: translateY(0) rotate(0deg); }
  50% { transform: translateY(-12px) rotate(8deg); }
}
```

#### Entrada da Página (RSVP)
```css
@keyframes fadeUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}
```

#### Hover nos Botões
- Transform: `translateY(-2px)`
- Box-shadow elevado
- Mudança de cor suave

---

## 📱 Responsividade

### Breakpoints

O design é **mobile-first** e se adapta automaticamente a diferentes tamanhos de tela:

```css
/* Smartphones */
@media (max-width: 480px) {
  - Nome: 72px → 64px
  - Padding reduzido: 56px → 40px
  - Corações decorativos removidos
  - Stepper de quantidade otimizado
}

/* Tablets */
@media (max-width: 768px) {
  - Layout de coluna única
  - Botões em full-width
}

/* Desktop */
@media (min-width: 769px) {
  - Layout otimizado para largura máxima
  - Efeitos hover ativos
}
```

### Otimização Mobile

- Viewport configurado: `width=device-width, initial-scale=1.0`
- Touch targets ≥ 44x44px
- Fontes legíveis em telas pequenas
- Scroll suave e natural

---

## ⚡ Otimizações

### Performance

- ✅ **Sem dependências externas** (apenas Google Fonts)
- ✅ **CSS inline** para Critical CSS
- ✅ **SVG inline** (sem requisições HTTP extras)
- ✅ **Preconnect** para Google Fonts
- ✅ **Animações GPU-accelerated** (transform/opacity)

### SEO e Compartilhamento

```html
<!-- Meta tags básicas -->
<meta name="description" content="..." />

<!-- Open Graph para WhatsApp/Facebook -->
<meta property="og:title" content="..." />
<meta property="og:description" content="..." />
<meta property="og:type" content="website" />
```

### Acessibilidade

- ✅ Semântica HTML5 correta
- ✅ Labels associados aos inputs
- ✅ Contraste de cores adequado (WCAG AA)
- ✅ Foco visível em elementos interativos
- ✅ Textos alternativos para SVGs decorativos

### Compatibilidade

| Navegador | Versão Mínima | Suporte |
|-----------|---------------|---------|
| Chrome | 60+ | ✅ Completo |
| Firefox | 55+ | ✅ Completo |
| Safari | 11+ | ✅ Completo |
| Edge | 79+ | ✅ Completo |
| Opera | 47+ | ✅ Completo |
| Mobile Safari | iOS 11+ | ✅ Completo |
| Chrome Mobile | Android 5+ | ✅ Completo |

---

## 📊 Recursos Técnicos Avançados

### JavaScript Interativo (RSVP)

#### Stepper de Quantidade de Acompanhantes

```javascript
// Incremento/Decremento com limites (0-20)
function changeQty(delta) {
  const input = document.getElementById('acompanhantes');
  let val = parseInt(input.value) || 0;
  val = Math.max(0, Math.min(20, val + delta));
  input.value = val;
}
```

#### Controle de Visibilidade Condicional

```javascript
// Mostrar campos de fralda apenas se confirmar presença
function toggleFraldaField() {
  const confirmaSim = document.getElementById('confirmaSim').checked;
  const fraldaSection = document.getElementById('fraldaSection');
  
  if (confirmaSim) {
    fraldaSection.classList.add('visible');
    document.getElementById('tamanho_fralda').required = true;
  } else {
    fraldaSection.classList.remove('visible');
    document.getElementById('tamanho_fralda').required = false;
  }
}
```

### CSS Grid para Layout de Formulário

```css
.radio-group {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px;
}
```

### Validação HTML5

```html
<input type="text" id="nome" required />
<input type="tel" id="telefone" placeholder="+55 (00) 00000-0000" required />
<textarea id="observacoes" maxlength="500"></textarea>
```

---

## 🐛 Solução de Problemas

### Google Forms não carrega

**Problema:** Iframe do Google Forms aparece em branco
**Solução:** 
1. Verifique se a URL está correta
2. Certifique-se de que o formulário está configurado para "Aceitar respostas"
3. Teste a URL do Forms diretamente no navegador

### Fontes não carregam

**Problema:** Fontes aparecem como padrão do sistema
**Solução:**
1. Verifique a conexão com internet
2. Confirme que o link do Google Fonts está correto (linhas 14-16)
3. Use fallback fonts (já configurado): `font-family: 'Great Vibes', cursive;`

### Layout quebrado no mobile

**Problema:** Elementos sobrepostos ou cortados
**Solução:**
1. Limpe o cache do navegador
2. Verifique se o viewport meta tag está presente: `<meta name="viewport" content="width=device-width, initial-scale=1.0" />`
3. Teste em modo de desenvolvedor do navegador

---

## 📝 Licença e Créditos

### Autor

Desenvolvido para o Chá de Fralda da Luiza

### Recursos Utilizados

- **Ícones:** SVG inline customizados
- **Fontes:** Google Fonts (SIL Open Font License)
- **Inspiração de Design:** Temas florais e lavanda

### Licença

Este projeto é de uso pessoal. Sinta-se livre para adaptar para seus próprios eventos.

---

## 🎉 Mensagem Final

> *"Com muito carinho, convidamos você para ajudar a mamãe e o papai a ganhar muitas fraldinhas pra Luiza! 💜"*

**Pedido:** Um pacote de fraldas por adulto
**Marcas sugeridas:** Huggies Supreme Care ou Pampers Premium Care
**Tamanho:** M

*P.S.: Fique à vontade para levar seu cooler com sua bebida alcoólica! 🍹*

---

**Dúvidas ou sugestões?** Este README cobre todos os aspectos técnicos do projeto, mas se precisar de mais informações, não hesite em entrar em contato!

---

✨ **Feito com 💜 para a Luiza**
