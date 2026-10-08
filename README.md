# Aconchego

Site estático acadêmico de uma ONG fictícia, desenvolvido com HTML5 semântico, CSS3 e JavaScript puro. A identidade, os textos e as imagens ilustrativas originais foram preservados sempre que estavam válidos.

## Como executar

1. Baixe ou clone o projeto.
2. Abra [`index.html`](./index.html) diretamente em um navegador moderno.
3. Navegue pelas três páginas pelo menu. Não há instalação de dependências, servidor, backend ou banco de dados.

## Estrutura

- [`index.html`](./index.html): apresentação institucional, equipe, galeria, notícias, transparência e newsletter demonstrativa.
- [`projetos.html`](./projetos.html): projetos, indicadores, voluntariado, doação demonstrativa e aviso sobre a mídia pendente.
- [`cadastro.html`](./cadastro.html): formulário semântico de apoiadores e voluntários, com validação nativa e resposta simulada.
- [`css/estilo.css`](./css/estilo.css): variáveis, paleta, Grid de 12 colunas, Flexbox, componentes e breakpoints responsivos.
- [`js/script.js`](./js/script.js): navegação, máscaras, validações complementares, newsletter e doação demonstrativa.
- [`img/`](./img/): novo logotipo PNG e imagens JPG ilustrativas.

## Funcionalidades JavaScript

- O menu hambúrguer e o submenu funcionam por clique e teclado. `aria-expanded`, `hidden` e `aria-controls` acompanham o estado visual.
- CPF, telefone e CEP recebem pontuação durante a digitação. O atributo `pattern` apenas verifica o formato final; ele não insere pontuação automaticamente nem comprova a validade real de um CPF.
- O cadastro usa a validação nativa do HTML. Ao enviar um formulário válido, impede a requisição inexistente e informa o nome, deixando claro que os dados não foram enviados nem salvos.
- A newsletter valida o e-mail pelo tipo `email` e exibe uma confirmação demonstrativa.
- A doação aceita um valor predefinido **ou** “Outro valor”, calcula a projeção de 12 meses para doações mensais e abre um modal de confirmação. Nenhum pagamento é realizado.

Os complementos pontuais em relação aos exemplos introdutórios da Aula 05 são `addEventListener`, `preventDefault`, `classList`, `hidden`, `textContent`, `checkValidity` e a conversão com `Number.parseFloat`. Eles conectam os conceitos de variáveis, funções, condicionais, strings e operações à interface sem adicionar bibliotecas.

## Aulas e conceitos aplicados

| Recurso | Conceito | Aula |
|---|---|---|
| `header`, `nav`, `main`, `section`, `article`, `footer` | HTML semântico e estrutura | Aula 01 e Aula 02 |
| Labels, fieldsets, legend, tipos de input e validação nativa | Formulários HTML5 | Aula 02 |
| Imagens responsivas e seção reservada para vídeo | Multimídia e carregamento responsável | Aula 03 |
| Variáveis CSS, seletores, estados e modelo de caixas | CSS externo e fundamentos de CSS | Aula 03 |
| Grid de 12 colunas e Flexbox | Layouts bidimensionais e alinhamento | Aula 04 |
| Menu responsivo, dropdown, cards, badges/alertas, toast e modal | Componentes e navegação | Aula 04 |
| `const`, `let`, funções, concatenação, conversão e cálculo | Fundamentos de JavaScript | Aula 05 |
| Eventos, DOM e `preventDefault` | Complemento necessário para interações | Aula 05 + complemento pontual |

## Limitações e pendências

- A pasta `media/` e os arquivos `aconchego.mp4`/`aconchego.webm` não foram entregues. Por isso, não foi inventado um vídeo nem mantido o iframe externo sem relação com o projeto; a página identifica a pendência e mantém uma imagem ilustrativa.
- As informações de cadastro, newsletter e doação são apenas demonstrações. Nenhum dado pessoal é colocado em `localStorage`, enviado a servidor ou persistido.
- As imagens existentes são JPG. A exigência de múltiplos formatos otimizados (como WebP) não é declarada como atendida, pois esses arquivos não foram fornecidos.
- O repositório público no GitHub é uma exigência da entrega acadêmica. Publique este diretório manualmente e preencha o link público quando o repositório existir; nenhuma visibilidade foi alterada automaticamente.
- Não foi realizada validação W3C, auditoria formal de acessibilidade ou publicação. Essas verificações permanecem pendentes.

## Testes recomendados

1. Abra cada página e teste os links do cabeçalho e rodapé.
2. Reduza a janela para conferir o menu hambúrguer, o submenu por clique e a navegação por `Tab`/`Escape`.
3. Na página de cadastro, tente enviar campos vazios ou inválidos e depois um cadastro completo; confira as máscaras e a mensagem com o nome.
4. Na newsletter, teste um e-mail inválido e um válido.
5. Na doação, teste valor predefinido, valor personalizado, valor vazio, valor menor que R$ 5, frequência mensal e cancelamento/confirmação do modal.
6. Confira as páginas em larguras aproximadas de 1200 px, 1000 px, 800 px, 600 px e 420 px.

Os testes acima são um roteiro manual. A conferência visual local e a leitura do código foram realizadas; validação automática, teste em leitores de tela e publicação ainda precisam ser feitos pelo estudante.

## Créditos das imagens

As fotografias foram baixadas de páginas do Pexels e são usadas como imagens ilustrativas. A licença indicada é a licença gratuita do Pexels, conforme as páginas de origem consultadas.

| Arquivo | Autor | Página de origem (URL) | Licença |
|---|---|---|---|
| `hero-comunidade.jpg` | cottonbro studio | https://www.pexels.com/photo/group-of-people-joining-hands-together-7322769/ | Licença Pexels |
| `equipe-1.jpg` | Ifeyinka Adeyemo | https://www.pexels.com/photo/professional-corporate-headshot-of-smiling-woman-29852895/ | Licença Pexels |
| `equipe-2.jpg` | Ernest Flowers | https://www.pexels.com/photo/professional-headshot-of-a-smiling-man-38677835/ | Licença Pexels |
| `equipe-3.jpg` | BULE | https://www.pexels.com/photo/natural-light-portrait-of-smiling-woman-35288344/ | Licença Pexels |
| `galeria-1.jpg` | Katerina Holmes | https://www.pexels.com/photo/anonymous-ethnic-tutor-helping-little-multiracial-students-with-task-in-classroom-5905492/ | Licença Pexels |
| `galeria-2.jpg` | Julia M Cameron | https://www.pexels.com/photo/people-packing-food-6995260/ | Licença Pexels |
| `galeria-3.jpg` | Ivan S | https://www.pexels.com/photo/people-putting-their-hands-together-9630204/ | Licença Pexels |
| `noticia-1.jpg` | Max Fischer | https://www.pexels.com/photo/a-children-clapping-together-5212700/ | Licença Pexels |
| `noticia-2.jpg` | Kampus Production | https://www.pexels.com/photo/man-and-woman-harvesting-at-a-vegetable-garden-7658779/ | Licença Pexels |
| `noticia-3.jpg` | Diva Plavalaguna | https://www.pexels.com/photo/group-of-people-joining-hands-6147373/ | Licença Pexels |
| `projeto-educacao.jpg` | Max Fischer | https://www.pexels.com/photo/students-listening-in-class-5427996/ | Licença Pexels |
| `projeto-alimentacao.jpg` | Julia M Cameron | https://www.pexels.com/photo/volunteers-giving-out-meals-wearing-face-masks-6995298/ | Licença Pexels |
| `projeto-renda.jpg` | Mehmet Turgut Kirkgoz | https://www.pexels.com/photo/women-working-in-a-workshop-11359621/ | Licença Pexels |
| `cadastro-voluntarios.jpg` | Tahir Xəlfəquliyev | https://www.pexels.com/photo/group-of-hands-showing-unity-and-teamwork-33963829/ | Licença Pexels |
