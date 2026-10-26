# Portfólio pessoal — HTML e CSS

> Projeto de estudo de uma página de portfólio para apresentação profissional, com navegação por seções, área de apresentação, seção “Sobre”, galeria de projetos e rodapé.

![Status](https://img.shields.io/badge/status-protótipo%20de%20estudo-blue)
![HTML5](https://img.shields.io/badge/HTML5-estrutura-orange)
![CSS3](https://img.shields.io/badge/CSS3-estilização-blue)
![JavaScript](https://img.shields.io/badge/JavaScript-não%20utilizado-lightgrey)

---

## 📋 Sobre o projeto

Este projeto consiste em um portfólio estático desenvolvido com **HTML5 e CSS3**, voltado ao estudo de estruturação semântica, composição visual, navegação por âncoras, efeitos de interação com CSS e adaptação do layout a diferentes larguras de tela.

A página apresenta uma seção inicial (*hero*), uma área sobre o profissional, uma galeria de imagens de projetos e um rodapé. O CSS utiliza Flexbox para organizar os elementos, transições para efeitos visuais e uma media query para ajustar partes do layout em telas menores.

### Objetivos de aprendizagem

- Praticar a organização de uma página HTML em seções.
- Aplicar estilos, cores, tipografia, espaçamento e imagens de fundo com CSS.
- Criar navegação interna usando links de âncora.
- Utilizar Flexbox para alinhamento e distribuição de conteúdo.
- Aplicar estados `:hover`, transições e rolagem suave.
- Introduzir regras de responsividade com `@media`.
- Organizar recursos estáticos em uma estrutura simples de diretórios.

## ✨ Recursos implementados

- [x] Menu superior fixo durante a rolagem (*sticky*).
- [x] Links internos para as seções Home, Sobre e Projetos.
- [x] Seção inicial com imagem de fundo e chamada para ação.
- [x] Seção de apresentação com texto e imagem.
- [x] Galeria visual de projetos com efeito de opacidade ao passar o cursor.
- [x] Rodapé com identificação do autor.
- [x] Rolagem suave entre as seções.
- [x] Ajustes de layout em telas com largura de até 1050 px.
- [ ] Links funcionais para cada projeto da galeria.
- [ ] Botão de orçamento conectado a e-mail, formulário ou outro canal de contato.
- [ ] Conteúdo biográfico e identificação profissional definitivos.

## 🖥️ Seções da página

| Seção | Identificador | Descrição |
|---|---|---|
| Home | `#home` | Apresentação inicial e link para a galeria. |
| Sobre | `#sobre` | Texto de apresentação acompanhado de uma imagem. |
| Projetos | `#projetos` | Galeria de imagens ilustrativas de projetos e botão de orçamento. |
| Rodapé | — | Nome ilustrativo e aviso de direitos reservados. |

## 🧰 Tecnologias e recursos

- **HTML5:** estrutura e conteúdo da página.
- **CSS3:** layout, cores, tipografia, transições e responsividade.
- **Flexbox:** alinhamento do menu, das seções e da galeria.
- **Google Fonts — Roboto:** tipografia carregada externamente; se não houver conexão, o navegador usa uma fonte sans-serif alternativa.
- **JavaScript:** não utilizado nesta versão.

## 📁 Estrutura do projeto

```text
fe_portifolio/
├── index.html
├── styles.css
├── README.md
└── images/
    ├── foto-pc.png
    ├── programador.png
    ├── projeto1.png
    ├── projeto2.png
    └── projeto3.png
```

## ▶️ Como executar

O projeto não exige instalação de dependências nem processo de compilação.

### Opção 1 — Abrir diretamente

1. Baixe ou clone o repositório.
2. Abra a pasta do projeto.
3. Abra o arquivo `index.html` em um navegador atualizado.

### Opção 2 — Executar pelo VS Code

1. Abra a pasta do projeto no Visual Studio Code.
2. Abra o arquivo `index.html`.
3. Use uma extensão de servidor local, como **Live Server**, se desejar atualizar a página automaticamente durante a edição.

### Clonar o repositório

```bash
git clone https://github.com/pratesddev/fe_portifolio.git
cd fe_portifolio
```

Depois, abra `index.html` no navegador ou inicie um servidor local pelo editor.

## 🧪 Checklist de validação

- [ ] O menu leva às seções corretas.
- [ ] A imagem de fundo e as imagens da pasta `images/` carregam corretamente.
- [ ] O botão “Veja meus projetos” leva à seção de projetos.
- [ ] Os efeitos de `:hover` funcionam com mouse e não são essenciais para compreender o conteúdo.
- [ ] A página permanece utilizável em telas estreitas e em zoom ampliado.
- [ ] O texto, os nomes e as imagens de exemplo foram substituídos por conteúdo real antes da publicação.
- [ ] Os botões e links que sugerem contato ou acesso a projetos possuem destinos funcionais.

## ⚠️ Limitações conhecidas

- O título da página, o texto do rodapé e parte do conteúdo ainda usam o nome ilustrativo **“Fulano de Tal”**; a seção “Sobre” contém texto de preenchimento.
- As imagens da galeria são exibidas como imagens estáticas e se repetem nas duas linhas. Elas não possuem links para páginas de projetos ou repositórios.
- O botão “Faça um orçamento” não tem ação implementada.
- O botão principal está dentro de um link. Para melhorar a semântica e a acessibilidade, prefira estilizar diretamente o próprio elemento `<a>` como botão, em vez de aninhar um `<button>` dentro dele.
- A regra responsiva atual cobre apenas alguns ajustes. O menu e a galeria merecem testes adicionais em celulares e tablets.
- O CSS remove o contorno padrão com `outline: 0`; é importante fornecer um indicador de foco visível para navegação por teclado.
- A imagem `foto-pc.png` possui o texto alternativo “Foto minha programando”, mas o nome do arquivo e a descrição devem ser revistos conforme o conteúdo real da imagem e a finalidade dela.
- A fonte Roboto depende de um serviço externo para ser carregada na versão atual.

## 🗺️ Próximas melhorias sugeridas

1. Substituir os textos de exemplo por uma apresentação profissional real.
2. Transformar cada item da galeria em um cartão com título, descrição, tecnologias utilizadas e links para demonstração e repositório.
3. Implementar o botão de orçamento com um canal de contato real.
4. Melhorar a responsividade com ajustes específicos para celular, tablet e desktop.
5. Corrigir a hierarquia semântica e revisar acessibilidade: foco visível, contraste, textos alternativos e uso por teclado.
6. Revisar o uso de elementos semânticos, incluindo um `<header>`, um `<main>` e uma estrutura de navegação com rótulo acessível.
7. Validar o HTML e testar a página em diferentes navegadores e tamanhos de tela.
8. Considerar metadados de compartilhamento e descrição da página antes de publicá-la.

## 👤 Autor

**Diego Prates**

- GitHub: [@pratesddev](https://github.com/pratesddev)
- LinkedIn: [Diego Prates](https://linkedin.com/in/prates-diego)
- E-mail: [dmoprates1@gmail.com](mailto:dmoprates1@gmail.com)
- Site: [ation.dev.br](https://ation.dev.br)

---

Desenvolvido como projeto de estudo de HTML e CSS.
