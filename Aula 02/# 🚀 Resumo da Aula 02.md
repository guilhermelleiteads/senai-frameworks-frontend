🚀 Resumo Completo – Configuração do Ambiente de Desenvolvimento (Frameworks Front-end)
📋 Visão Geral

Esta aula apresenta os conceitos fundamentais para configurar um ambiente de desenvolvimento moderno para aplicações Front-end, abordando:

🔄 Versionamento de software
🏷️ Versionamento Semântico (SemVer)
🌿 Git e GitHub
🛠️ Visual Studio Code (VS Code)
⚡ Node.js e NPM
⚛️ Criação de projetos React
☁️ Deploy utilizando Vercel
🔄 Introdução ao Versionamento

O versionamento é o processo de controlar e registrar alterações realizadas em arquivos e projetos de software ao longo do tempo.

✅ Principais benefícios
📜 Histórico Completo

Permite acompanhar todas as alterações realizadas.

👤 Rastreabilidade

Identifica:

Quem alterou
Quando alterou
O que foi alterado
Motivo da alteração
🤝 Colaboração Segura

Vários desenvolvedores podem trabalhar simultaneamente no mesmo projeto.

⏪ Recuperação de Versões

Possibilita retornar a versões estáveis em caso de erros.

💾 Versionamento x Backup
Versionamento	BackupHistórico completo	Apenas cópia do estado atual
Registro de autoria	Não registra autores
Colaboração simultânea	Não suporta colaboração
Recuperação granular	Recuperação total
Controle de mudanças	Apenas armazenamento
🚨 Problemas sem Versionamento
📁 Arquivos duplicados
❌ Perda de código
⚔️ Conflitos entre desenvolvedores
🔍 Falta de histórico

Exemplo clássico:

projeto-final.zip
projeto-final-agora-vai.zip
projeto-final-definitivo.zip
projeto-final-definitivo-agora-sim.zip

🏷️ Versionamento Semântico (SemVer)

O Semantic Versioning (SemVer) define versões seguindo o padrão:

MAJOR.MINOR.PATCH


Exemplo:

2.1.3

📊 Estrutura do SemVer
🔴 MAJOR (2.0.0)

Mudanças incompatíveis com versões anteriores.

Exemplo:

1.0.0 → 2.0.0

🟡 MINOR (1.1.0)

Novas funcionalidades sem quebrar compatibilidade.

Exemplo:

1.0.0 → 1.1.0

🟢 PATCH (1.0.1)

Correções de bugs sem alterar funcionalidades.

Exemplo:

1.0.0 → 1.0.1

📌 Exemplos Práticos
Versão	Significado1.0.0	Primeira versão estável
1.1.0	Nova funcionalidade
1.1.1	Correção de bug
2.0.0	Mudança incompatível
🔧 Tipos de Alterações no Código
🐞 Bug Fix
✨ Nova Funcionalidade
🔨 Refatoração
🚀 Melhoria de Performance
🔐 Correções de Segurança
📦 Atualização de Dependências
✅ Inclusão de Testes
🌿 Git
📖 O que é Git?

Git é um sistema de controle de versão distribuído criado para acompanhar mudanças em projetos de software.

Principais funções
📌 Registrar versões
📂 Armazenar histórico
🔄 Compartilhar código
👥 Facilitar trabalho em equipe
⏪ Restaurar versões anteriores
⚙️ Instalação do Git
Passos

Baixar em:

https://git-scm.com/downloads

Executar o instalador

Seguir:

Next → Next → Install

Testar instalação:
git --version

👤 Configuração Inicial

Após instalar:

git config --global user.name "Seu Nome"

git config --global user.email "seuemail@email.com"

🏷️ Tags no Git

Tags servem para marcar versões importantes do projeto.

Exemplo:

git tag 1.0.0


Enviar para o GitHub:

git push origin 1.0.0

Tipos de Tags
⚡ Lightweight

Apenas um nome associado a um commit.

📝 Annotated

Contém:

Autor
Data
Mensagem
Metadados adicionais
✅ Boas Práticas com Git
📌 Commits Pequenos

Faça commits frequentes.

✅ Facilita correções.

📝 Mensagens Claras

Exemplos:

feat: adicionar tela de login

fix: corrigir erro na validação

🌿 Uso de Branches

Criar branches para:

Novas funcionalidades
Correções
Testes

Mantendo a branch principal estável.

✅ Testes Antes do Merge

Sempre validar o código antes de integrar mudanças.

🛠️ IDE e Visual Studio Code
O que é uma IDE?

IDE significa:

Integrated Development Environment

É um ambiente que reúne:

Editor de código
Compilador
Depurador
Ferramentas de teste
Integração com Git
💻 Visual Studio Code

O VS Code é um editor leve que pode se tornar uma IDE completa através de extensões.

Benefícios
🚀 Leve
⚙️ Altamente personalizável
🔌 Grande biblioteca de extensões
🌿 Integração com Git
⚛️ Excelente suporte ao React
⚡ Node.js
O que é?

Node.js é um ambiente que permite executar JavaScript fora do navegador.

Vantagens
Utilizar JavaScript no backend
Alto desempenho
Grande ecossistema
Integração com aplicações Front-end
Instalação

Baixar em:

https://nodejs.org


Verificar instalação:

node --version

📦 NPM (Node Package Manager)

O NPM é instalado junto com o Node.js.

Funções
Instalar bibliotecas
Atualizar pacotes
Gerenciar dependências
Compartilhar módulos
package.json

Arquivo responsável por armazenar:

Dependências
Scripts
Informações do projeto
Configurações
Instalar dependências
npm install


ou

npm i

⚛️ Criando um Projeto React
Comando
npx create-react-app meu-projeto-react

O que é criado?

✅ Configuração pronta

✅ Webpack

✅ Babel

✅ Ambiente de desenvolvimento

✅ Estrutura de pastas

✅ Scripts prontos

Passo a Passo
1️⃣ Criar o projeto
npx create-react-app meu-projeto-react

2️⃣ Acessar a pasta
cd meu-projeto-react

3️⃣ Abrir no VS Code
code .

4️⃣ Executar projeto
npm start

📁 Estrutura do Projeto React
node_modules

📦 Dependências instaladas.

public

🌐 Arquivos públicos:

HTML
JSON
Imagens
src

💻 Código-fonte da aplicação.

Arquivos importantes
index.js

Ponto de entrada da aplicação.

App.js

Componente principal.

App.css

Estilos específicos do App.

index.css

Estilos globais.

.gitignore

Define arquivos ignorados pelo Git.

Exemplo:

node_modules/
.env

☁️ Deploy
O que é Deploy?

Deploy é o processo de publicar uma aplicação para que usuários possam acessá-la.

Etapas
Compilar código
Configurar ambiente
Executar testes
Publicar aplicação
☁️ Vercel

A Vercel é uma plataforma especializada em hospedagem e deploy de aplicações modernas.

Principais Recursos
🔗 Integração com Git

Conecta-se diretamente com:

GitHub
GitLab
Bitbucket
🚀 Deploy Automático

Cada push pode gerar uma nova publicação automaticamente.

⏪ Rollback

Permite retornar para versões anteriores.

⚡ CDN Global

Distribuição rápida de conteúdo no mundo inteiro.

☁️ Serverless Functions

Execução de backend sem gerenciar servidores.

📈 Escalabilidade Automática

Capacidade de crescer conforme o aumento da demanda.

🎯 Fluxo Completo de Desenvolvimento
graph LR
A[VS Code] --> B[React]
B --> C[Git]
C --> D[GitHub]
D --> E[Vercel]
E --> F[Aplicação Online]

📝 Atividade Proposta

Desenvolver uma aplicação React seguindo o fluxo:

⚛️ Criar projeto React
💻 Desenvolver no VS Code
🌿 Versionar utilizando Git
📤 Enviar para GitHub
☁️ Publicar na Vercel
🌍 Disponibilizar URL pública
🎓 Conclusão

Esta aula apresentou todo o ecossistema necessário para desenvolver aplicações Front-end modernas. O aluno aprende a configurar seu ambiente utilizando VS Code, Git, Node.js, NPM e React, além de aplicar boas práticas de versionamento e realizar o deploy automatizado na Vercel, reproduzindo um fluxo profissional amplamente utilizado no mercado de desenvolvimento web.
