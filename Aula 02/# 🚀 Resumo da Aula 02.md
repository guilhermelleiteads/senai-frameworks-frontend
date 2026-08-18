# 🚀 Resumo Completo – Configuração do Ambiente de Desenvolvimento (Frameworks Front-end)

## 📋 Visão Geral

Esta aula apresenta os conceitos fundamentais para configurar um ambiente de desenvolvimento moderno para aplicações Front-end, abordando:

- 🔄 Versionamento de software
- 🏷️ Versionamento Semântico (SemVer)
- 🌿 Git e GitHub
- 🛠️ Visual Studio Code (VS Code)
- ⚡ Node.js e NPM
- ⚛️ Criação de projetos React
- ☁️ Deploy utilizando Vercel

---

# 🔄 Introdução ao Versionamento

O **versionamento** é o processo de controlar e registrar alterações realizadas em arquivos e projetos de software ao longo do tempo.

## ✅ Principais Benefícios

### 📜 Histórico Completo
Permite acompanhar todas as alterações realizadas durante o desenvolvimento do projeto.

### 👤 Rastreabilidade
Possibilita identificar:

- Quem realizou a alteração
- Quando a alteração foi feita
- O que foi modificado
- Qual foi o motivo da mudança

### 🤝 Colaboração Segura
Diversos desenvolvedores podem trabalhar simultaneamente no mesmo projeto sem sobrescrever o trabalho dos colegas.

### ⏪ Recuperação de Versões
Permite retornar a versões anteriores de forma segura caso ocorram erros ou falhas.

---

## 💾 Versionamento x Backup

| Versionamento | Backup |
|-------------|---------|
| Histórico completo de alterações | Apenas uma cópia do estado atual |
| Registro de autoria | Não registra autores |
| Colaboração simultânea | Não suporta colaboração |
| Recuperação granular | Recuperação completa |
| Controle de mudanças | Apenas armazenamento |

### 🚨 Problemas Sem Versionamento

- 📁 Arquivos duplicados
- ❌ Perda de código
- ⚔️ Conflitos entre desenvolvedores
- 🔍 Ausência de histórico

### Exemplo Clássico

```text
projeto-final.zip
projeto-final-agora-vai.zip
projeto-final-definitivo.zip
projeto-final-definitivo-agora-sim.zip
