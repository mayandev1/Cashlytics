# Cashlytics

> Um dashboard financeiro moderno focado em visualização de dados e experiência do usuário.

O **Cashlytics** é uma aplicação web desenvolvida com **HTML, CSS e JavaScript puro**, projetada para controle financeiro pessoal com uma interface estilo fintech e foco em análise de dados.

## ✨ Demonstração

🔗 Acesse: https://dashboardcashlytics.netlify.app/

## 🧠 Sobre o projeto

Este projeto foi desenvolvido com o objetivo de:

- Praticar manipulação de dados no front-end
- Trabalhar com visualização de dados (gráficos)
- Simular um sistema real de controle financeiro
- Criar um projeto relevante para portfólio (foco em dados)

## ⚙️ Tecnologias utilizadas

- HTML5
- CSS3 (com variáveis e animações)
- JavaScript (Vanilla ES2020)
- Chart.js (visualização de dados)
- jsPDF + jsPDF-AutoTable (geração de extratos em PDF)
- localStorage (persistência de dados)

## 📊 Funcionalidades

### 👤 Perfil do usuário (New Feature)
- Tela de boas-vindas com design premium na primeira visita
- Campo para inserir o nome do titular
- Nome salvo localmente — não é solicitado novamente nas próximas visitas
- Chip com inicial e primeiro nome exibido no header
- Opção de renomear a qualquer momento clicando no chip

### 💸 Transações
- Adicionar receitas e despesas com toggle visual por tipo
- Categorizar transações (Alimentação, Transporte, Saúde, Salário, Freelance, etc.)
- Excluir transações
- Validação de dados com feedback visual via toasts

### 📈 Dashboard
- Saldo total com indicador positivo/negativo
- Total de receitas e despesas
- Atualização dinâmica com animação de contagem

### 📉 Visualização de dados
- Gráfico de rosca (despesas por categoria)
- Gráfico de barras (receitas vs despesas no período)

### 🔍 Filtros
- Por mês
- Por tipo (receita/despesa)
- Limpeza rápida de filtros

### 📄 Extrato em PDF (New Feature)
- Botão "Extrato PDF" no header, acessível em mobile e desktop
- Modal com seletor de período (data início → data fim)
- Preview em tempo real: transações, entradas, saídas e saldo antes de gerar
- PDF com tema escuro no padrão visual do app, contendo:
  - Logo e nome do app no cabeçalho
  - Nome do titular e período selecionado
  - Cards de resumo (entradas, saídas, saldo)
  - Transações agrupadas por data com saldo do dia
  - Chip de categoria em cada transação
  - Resumo final consolidado
  - Rodapé com número de página
- Nome do arquivo gerado automaticamente por titular e período

### 💾 Persistência
- Dados salvos no navegador com `localStorage`
- Perfil do usuário salvo separadamente das transações

## 🎨 Interface

- Tema escuro (dark mode) com acento lime elétrico
- Design inspirado em fintechs modernas
- Layout responsivo (mobile + desktop)
- Animações com `translate3d` na GPU (fluido em 120fps)
- Feedback visual em todas as interações
- Grain texture sutil no fundo
- Tipografia: Syne (display) + DM Sans (corpo) + JetBrains Mono (valores)

## 📂 Estrutura do projeto

```

cashlytics/
│
├── index.html       # Aplicação completa (HTML + CSS + JS em arquivo único)
└── README.md        # Este arquivo

````

## ▶️ Como executar

1. Clone o repositório:

```bash
git clone https://github.com/mayandev1/cashlytics.git
````

2. Abra o arquivo:

```
index.html
```

> Não precisa de servidor, build ou instalação. Abre direto no navegador.

## ⚖️ Prós e Contras

### ✅ Prós

* Interface moderna e profissional
* Código simples e direto (sem frameworks)
* Uso eficiente de `localStorage`
* Boa base para evoluir para aplicações maiores
* Visualização de dados clara e útil
* Extrato em PDF personalizável por período
* Projeto forte para portfólio (especialmente área de dados)
* Otimizado para 120fps com `will-change`, `contain` e `translate3d`

### ❌ Contras

* Dados limitados ao navegador (não sincroniza entre dispositivos)
* Sem sistema de login/autenticação
* Não permite edição de transações (apenas exclusão)
* Dependência de CDN (Chart.js, jsPDF)
* Escalabilidade limitada sem backend

## 🛠️ Melhorias futuras

* ✏️ Edição de transações
* 📤 Exportar/importar dados (JSON/CSV)
* 🔁 Transações recorrentes
* 🎯 Metas de orçamento por categoria
* 🌐 Suporte a múltiplas moedas
* 🎨 Alternância de tema (dark/light)
* ☁️ Integração com backend + autenticação
* 👤 Cadastro completo do titular (quando houver backend)

## 📌 Aprendizados

Durante o desenvolvimento deste projeto, foram trabalhados conceitos como:

* Manipulação de estado no JavaScript
* Estruturação de código sem frameworks
* Visualização de dados com gráficos
* Organização de UI/UX
* Persistência de dados no navegador
* Geração de PDFs client-side com jsPDF
* Otimização de performance para telas de alta taxa de atualização

## 👨‍💻 Autor

Desenvolvido por **Mayan Gabriel**
🔗 [https://github.com/mayandev1]

## 📄 Licença

Este projeto está sob a licença MIT.