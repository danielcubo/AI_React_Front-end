## 1. Por que foi necessária a criação do React?

O React foi criado pelo Facebook (atualmente Meta) e lançado em 2013 para resolver um problema muito específico: **a complexidade e a lentidão em atualizar interfaces dinâmicas em larga escala.**

Antes do React, a manipulação da tela era feita diretamente no **DOM (Document Object Model)** do navegador usando JavaScript puro ou jQuery. Quando o Facebook começou a crescer muito (pense no feed de notícias, chat abrindo, notificações subindo, curtidas atualizando em tempo real), aconteceram dois grandes problemas:

1. **Gargalo de Performance:** Atualizar o DOM diretamente é uma operação muito "cara" e lenta para o navegador. Mudar múltiplos elementos ao mesmo tempo causava travamentos na tela.
2. **Inconsistência de Estado:** Era muito difícil garantir que os dados no servidor fossem exatamente os mesmos que o usuário estava vendo na tela se várias interações acontecessem ao mesmo tempo.

### A Solução do React: O Virtual DOM e Componentização

O React revolucionou o desenvolvimento web ao introduzir dois conceitos chave:

* **Virtual DOM:** Em vez de atualizar a tela diretamente a cada clique, o React cria uma cópia leve da interface na memória (o Virtual DOM). Quando algo muda, ele calcula a forma mais rápida e eficiente de atualizar apenas o pedaço da tela que realmente mudou, poupando processamento.
* **Componentização:** Ele permitiu dividir a tela em pedaços isolados, reutilizáveis e independentes chamados componentes (um botão, um card de produto, uma barra de busca).

---

## 2. Onde o uso do React é Necessário (Ideal)?

Hã duas abordagens gerais para criar aplicativos web hoje: aplicativos Web tradicionais que executam a maior parte da lógica do aplicativo no servidor e SPAs (Single Page Applications) que executam a maior parte da interface do usuário no navegador, comunicando-se com o servidor Web principalmente usando APIs web. 

O React brilha em cenários onde a experiência do usuário precisa ser fluida, rápida e altamente interativa. Ele é altamente recomendado para:

* **Single Page Applications (SPAs):** Aplicações web onde o usuário navega por diferentes seções sem que a página precise recarregar do zero (ex: dashboards administrativos, painéis financeiros, Gmail).
* **Interfaces Altamente Dinâmicas:** Plataformas onde os dados mudam em tempo real na tela sem intervenção manual (ex: feeds de redes sociais como Instagram, chats, plataformas de streaming como Netflix).
* **Sistemas de Grande Porte Reutilizáveis:** Projetos onde times grandes trabalham juntos e precisam reutilizar os mesmos elementos de design (botões, modais, formulários) em várias partes do sistema.

---

## 4. Onde o uso do React NÃO é necessário?

Usar React para tudo é um erro comum de engenharia conhecido como *overengineering* (complexidade desnecessária). O uso dele dispensa-se em:

* **Sites Estáticos e Simples:** Blogs institucionais, portfólios simples, landing pages de marketing ou páginas de termos de uso. O HTML e CSS puros (com um toque de JavaScript básico) carregam muito mais rápido e são mais fáceis de manter nesses casos.
* **Páginas com Pouquíssima Interatividade:** Se a página serve apenas para exibir conteúdo de texto e imagens, carregar toda a estrutura do React para o navegador do usuário é um desperdício de desempenho e banda.
* **Projetos com Restrição Crítica de Tamanho de Arquivo:** O React adiciona um peso inicial de bytes (o *bundle size*) ao projeto. Para microssites extremamente otimizados para redes móveis precárias, soluções mais leves (ou JavaScript puro) são melhores.

## Alterar o Estado

## Hooks
Gerencia o estado e os ciclos de vida dentro de funções simples
- `useState`
- `useEffect`

## Closures

