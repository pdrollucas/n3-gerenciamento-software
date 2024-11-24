# N3 - Gerenciamento de Software

**Curso**: Engenharia de Software  
**Disciplina**: Gerenciamento, Configuração e Processos de Software  
**Professor**: Ricardo  
**Aluno**: Pedro Lucas Luckow  

---

## Objetivo do Projeto

Implementar um controle de versão eficiente, alinhado às normas de gestão de configuração da MPS-BR.

---

## Requisitos do Trabalho

1. Crie um repositório no GitHub.  
2. Crie as estórias de usuário.  
3. Defina seu fluxo de trabalho no Git.  
4. Crie um arquivo `.gitignore`.  
5. Defina os itens de configuração.  
6. Estabeleça uma estratégia para tags e liberação de releases.  

---

## Estratégias de Desenvolvimento

- O trabalho foi realizado de forma individual.  
- Como o foco da disciplina são as boas práticas do Git e GitHub, não me importei com o desenvolvimento de código.  
- Nesse trabalho, utilizei commits, pull requests, merges, branches, tags e releases. Também utilizei a parte de issues para a organização das atividades a serem realizadas.  
- Para poder utilizar todas essas funcionalidades sem o desenvolvimento de um código, **usei o próprio README** para registrar alterações. Cada atualização em um requisito da atividade contém uma branch específica usada para o desenvolvimento e, consequentemente, uma release. É possível ver o README ser atualizado a cada branch e release. Tratei cada adição de requisitos como se fosse uma nova funcionalidade, por isso o **MINOR** das tags e releases é atualizado. Tratei cada ajuste de formatação no texto como se fosse um bug, por isso o **PATCH** é atualizado. Caso uma alteração envolvesse mais de uma seção e incluísse uma reformulação completa da formatação do texto, ela seria tratada como uma alteração de **MAJOR**.

---

## Estórias de Usuário

1. **Administrador de Configuração**:  
   _"Como administrador de configuração, quero configurar o repositório no GitHub para que as alterações sejam rastreadas e versionadas adequadamente."_  
2. **Desenvolvedor**:  
   _"Como desenvolvedor, quero utilizar um fluxo de trabalho padronizado no Git, para que o desenvolvimento seja organizado e as entregas controladas."_  
3. **Gestor**:  
   _"Como gestor, quero criar releases versionadas, para que o histórico de versões esteja alinhado às entregas do projeto."_

---

## Fluxo de Trabalho no Git

As branches seguem a seguinte organização:

- **Main**: branch principal, contendo o código estável e liberado.  
- **Develop**: branch utilizada como referência para o desenvolvimento de novas funcionalidades ou ajustes.  
- **Features/adicao-{descricao-da-nova-funcionalidade}**: branch para adicionar novas funcionalidades.  
- **Fix/{local-ajustado}**: branch para correção de defeitos.  

### Regras

- Branches **features** e **fix** derivam da branch `develop` e, após concluídas, passam por _pull requests_ antes de serem mescladas.  
- Alterações na branch `develop` só serão promovidas para a branch `main` após estabilidade e liberação.  
- Commits devem ser **claros**, **concisos** e **consistentes**.  

---

## Itens de Configuração

O projeto simula o uso de **Vue.js**, **Node.js**, **C#** e **SQL**. Os itens de configuração estão organizados da seguinte forma:

1. **Vue.js e Node.js**:  
   - **Código-fonte**: `src/`, `public/`  
   - **Configurações**: `package.json`, `*config.js`, `.env.example`  
2. **C#**:  
   - **Código-fonte**: `*.cs`, `*.csproj`, `*.sln`  
   - **Configurações**: `appsettings.json`  
3. **SQL**:  
   - **Scripts**: `/migrations/`, `/seeds/`, `schema.sql`  

---

## Estratégia para Tags e Liberação de Releases

O projeto adota o **Versionamento Semântico (SemVer)** no formato `MAJOR.MINOR.PATCH`.  

### Regras

- **MAJOR**: alterações incompatíveis que quebram a API.  
- **MINOR**: adição de novas funcionalidades compatíveis.  
- **PATCH**: correções de bugs e melhorias menores.  

### Exemplos de Versionamento

- `1.0.0`: primeira versão estável.  
- `1.1.0`: adição de nova funcionalidade compatível.  
- `1.1.1`: correção de bug ou melhoria menor na funcionalidade existente.  

Referência: [Versionamento Semântico - Dev do Futuro](https://www.devdofuturo.com/versionamento-semantico-o-que-e-e-como-aplicar)
