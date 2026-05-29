# 📚 Pequenos Leitores

> Plataforma web educativa para auxiliar crianças no processo de alfabetização em português.

---

## 🔗 Links Importantes

| | Link |
|---|---|
| 🌐 **Site publicado** | (https://pequenos-leitores.webflow.io) |
| 🎥 **Vídeo no YouTube** | (https://www.youtube.com/watch?v=Bkga1QX28Jg) |

---

## 📋 Sobre o Projeto

**Pequenos Leitores** é uma plataforma web educativa criada para auxiliar crianças no processo de alfabetização em português de forma simples, acessível e interativa. O site disponibiliza materiais educativos, conteúdos gratuitos e recursos de apoio para pais, responsáveis e professores que desejam ensinar crianças a ler em casa.

**Instituição:** UniFECAF — Faculdade de Inteligência Artificial  
**Autora:** Paloma Ai Tsuchinaga  
**Ano:** 2026  
**Disciplina:** Padrões Web para No-code e Low-code  

---

## 🎯 Público-Alvo

- Famílias e responsáveis
- Educadores e professores
- Crianças em fase inicial de aprendizagem da leitura
- Estudantes que necessitam de apoio complementar fora do ambiente escolar

---

## 🛠️ Ferramenta Utilizada

O projeto foi desenvolvido com **[Webflow](https://webflow.com/)**, uma plataforma **no-code** voltada para a criação de websites modernos e responsivos.

### Por que Webflow?

- Interface de arrastar e soltar intuitiva
- Suporte a animações e movimentos personalizados
- Padronização de estilos via variáveis de cor, tipografia e espaçamento
- Facilidade de manutenção futura, mesmo sem conhecimento técnico avançado
- Responsividade nativa para múltiplos tamanhos de tela

### ⚠️ Limitações Conhecidas

- Funcionalidades avançadas podem exigir conhecimentos em HTML, CSS ou JavaScript
- Alguns recursos estão restritos nos planos gratuitos
- A manutenção periódica de interações complexas pode demandar familiaridade com a ferramenta

---

## 📄 Páginas do Site

### 🏠 Home
Página principal da plataforma, com:
- Navbar de navegação
- Pop-up de cadastro de interessados
- Hero section com imagem e chamada para ação ("Começar Agora")
- Seção de citação (blockquote)
- Grade de conteúdos educativos com 4 módulos:
  - Alfabeto Fônico
  - Criando Sílabas
  - Pequenas Palavras
  - Aprendendo as Regras
- Footer

### 📝 Atividades
Página de materiais para download e prática, com:
- Navbar e pop-up
- Grade de apostilas organizadas por nível:
  - Workbook Pré 1
  - Workbook Pré 2
  - Workbook 1
  - Workbook 2
  - Workbook 3
  - Workbook 4
- Footer

---

## 🎨 Design System (CSS)

### Paleta de Cores

| Nome | Hex |
|---|---|
| Magenta | `#f7008b` |
| Fuchsia | `#e93bf8` |
| Shocking Pink | `#ea37ba` |
| Rose | `#e9357f` |
| Red Munsell | `#ea3348` |
| Red | `#eb3223` |
| Phlox | `#b14ef6` |
| Tropical Indigo | `#8082f8` |
| Deep Sky Blue | `deepskyblue` |
| Cyan | `#75fdfd` |
| Yellow | `#fef65c` |
| Mid Yellow | `#ffd301` |
| Dark Yellow | `#ffaa1c` |
| White | `#fdfdfd` |
| Light Gray | `#ededed` |
| Gray | `#ddd` |
| Dark Gray | `#9a9a9a` |
| Black | `#333` |
| Transparent | `rgba(255,255,255,0)` |
| Dark Transparent | `rgba(0,0,0,0.4)` |

### Tipografia

| Variável | Fonte |
|---|---|
| `sniglet` | Sniglet |
| `quicksand` | Quicksand |

### Border Radius

| Variável | Valor |
|---|---|
| `radius-16` | 16px |
| `radius-8` | 8px |
| `radius-4` | 4px |
| `radius-0` | 0px |

### Tamanhos de Texto (Fluid Typography com `clamp()`)

Todos os tamanhos utilizam a função CSS `clamp()` para escalonamento fluido entre telas pequenas e grandes:

| Elemento | Comportamento |
|---|---|
| H1 | Escala de ~1.5rem até ~4rem |
| H2 | Escala de ~1rem até ~3rem |
| H3 | Escala de ~1rem até ~2rem |
| Parágrafo | Escala de ~0.75rem até ~1rem |
| Quote | Escala de ~0.75rem até ~1.25rem |
| Footer Title | Escala até ~1.75rem |
| Footer Text | Escala até ~1rem |

---

## ⚙️ Funcionalidades e Interações (JavaScript / Webflow Interactions)

### Pop-up de Cadastro
O pop-up é o elemento de destaque do projeto em termos de implementação. Ele demonstra o uso de interações do Webflow equivalentes a comportamentos JavaScript:

- **Trigger:** Clique do mouse (tap)
- **Ação no 1º clique:** Inicia animação `open-popup` → exibe o pop-up com `Hide/Show`
- **Ação no 2º clique:** Fecha o pop-up com `close-popup`
- **Compatibilidade:** Desktop, Tablet, Mobile Landscape e Mobile Portrait
- **Configurações de CSS:** `position: fixed`, `display: flex`, alinhamento central nos eixos X e Y, largura e altura de 100%

---

## 📱 Responsividade

A plataforma foi adaptada para os seguintes breakpoints com o auxílio do **Fluid Builder**:

| Dispositivo | Largura aproximada |
|---|---|
| Desktop | 1148px+ |
| Tablet | 825px |
| Mobile L | 683px |
| Mobile P | 390px |

Ajustes realizados por breakpoint:
- Tamanho e escalonamento de textos
- Espaçamentos e margens dos elementos
- Largura dos blocos de conteúdo
- Reorganização do layout para telas menores
- Menu hambúrguer (`≡`) para navegação mobile

---

## ♿ Acessibilidade

Boas práticas adotadas no projeto:

- Cores com contraste adequado entre fundo e texto
- Fontes legíveis (Sniglet e Quicksand)
- Botões de fácil identificação visual
- Navegação simples e intuitiva
- Separação visual clara entre seções
- Evitou-se excesso de informações simultâneas na tela

---

## 📁 Estrutura do Projeto no Webflow

```
Body
└── page-wrapper
    ├── navbar (componente global)
    ├── pop-up (componente global)
    ├── hero-wrapper
    │   ├── image-wrapper-container
    │   └── Div Block 4
    │       ├── H1 title
    │       ├── Paragraph 2
    │       └── button-comecar
    ├── quote
    │   └── quote-container
    │       └── Block Quote
    ├── main-content
    │   ├── content-title
    │   │   ├── Heading 9
    │   │   ├── Heading 14
    │   │   └── Paragraph 3
    │   └── content-grid
    │       ├── alfabeto-fonico
    │       ├── criando-silabas
    │       ├── pequenas-palavras
    │       └── aprendendo-regras
    ├── footer (componente global)
    └── Section
```

---

## 💡 Aprendizados

> Ao utilizar o Webflow no desenvolvimento do projeto, ficou evidente que mesmo ferramentas no-code dependem dos padrões da web para funcionar corretamente. O processo possibilitou compreender melhor a estrutura HTML, a estilização via CSS e a aplicação de interações semelhantes ao JavaScript. Ferramentas no-code aceleram o desenvolvimento, mas ainda exigem lógica, planejamento e conhecimento básico sobre desenvolvimento web.

---

*Projeto acadêmico desenvolvido para a disciplina de Padrões Web para No-code e Low-code — UniFECAF, 2026.*
