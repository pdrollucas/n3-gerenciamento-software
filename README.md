# n3-gerenciamento-software
Curso: Engenharia de Software <br/>
Disciplina: Gerenciamento, configuração e processos de software <br/>
Professor: Ricardo <br/>
Aluno: Pedro Lucas Luckow <br/>

O foco do projeto será implementar um controle de versão eficiente, que atenda as normas de gestão de configuração da MPS-BR.
<ul>
  <li>Crie um repositório no github;</li>
  <li>Crie as estórias de usuário;</li>
  <li>Defina seu fluxo de trabalho no git;</li>
  <li>Crie um .gitignore;</li>
  <li>Defina os itens de configuração;</li>
  <li>Defina uma estratégia para tags e liberação de releases.</li>
</ul>

<hr/>
Estórias de usuário: 
<br/>
<br/>
<ul>
  <li>Como um administrador de configuração, eu quero configurar o repositório no GitHub, para que as alterações sejam rastreadas e versionadas adequadamente.<br/></li>
  <li>Como um desenvolvedor, eu quero utilizar um fluxo de trabalho padronizado no Git, para que o desenvolvimento seja organizado e as entregas controladas.</li>
  <li>Como um gestor, eu quero criar releases versionadas, para que o histórico de versões esteja alinhado às entregas do projeto.</li>
</ul>

<hr/>
Fluxo de trabalho no git
<br/>
<br/>
As branchs estão organizadas da seguinte forma:
<br/>
<br/>
<ul>
  <li>Main: branch principal, contendo o código estável e liberado</li>
  <li>Develop: branch utilizada como referência para o desenvolvimento de novas funcionalidades ou ajustes</li>
  <li>Features/adicao-{descricao da nova funcionalidade}: branchs responsáveis pela adição de novas funcionalidades</li>
  <li>Fix/{local ajustado}: branchs utilizadas para a correção de defeitos</li>
</ul>

Importante: as branchs de features e de fix sempre terão como referência a branch de develop, assim que tiverem resolvidas deverão realizar a pull request e depois o merge. A branch de main só puxará de develop quando esta estiver devidamente estável e liberada. Além disso, os commits realizados nas branchs de features e de fix deverão ser claros, consisos e consistentes. Antes de cada merge, haverá uma pull request responsável em garantir a revisão do código.

<hr/>
Itens de configuração
<br/>
<br/>
Simulando um cenário em que seria utilizado vue, node, c# e sql para o desenvolvimento do projeto...
<br/>
<br/>
<ol>
  <li>
    Vue.JS e Node.js:
    <ul>
      <li>Código-fonte: <code>src/</code>, <code>public/</code></li>
      <li>Configurações: <code>package.json</code>, <code>*config.js</code>, <code>.env.example</code></li>
    </ul>
  </li>
  <li>
    C#:
    <ul>
      <li>Código-fonte: <code>*.cs</code>, <code>*.csproj</code>, <code>*.sln</code></li>
      <li>Configurações: <code>appsettings.json</code></li>
    </ul>
  </li>
  <li>
    SQL:
    <ul>
      <li>Scripts: <code>/migrations/</code>, <code>/seeds/</code>, <code>schema.sql</code></li>
    </ul>
  </li>
</ol>

<hr/>
Estratégia para tags e liberação de releases:
<br/>
<br/>
Para esse projeto foi adotado um versionamento semântico (SemVer), com o formato MAJOR.MINOR.PATCH:
<ul>
  <li>MAJOR: alterações incompátiveis que quebrarão a API</li>
  <li>MINOR: novas funcionalidades compátiveis foram adicionadas</li>
  <li>PATCH: correções de bugs e pequenas melhorias</li>
</ul>
Exemplo: uma versão 1.0.0 terá o MAJOR como 1, o MINOR como 0 e o PATCH como 0. Uma versão 1.1.0, terá uma nova funcionalidade compátivel. Uma vesão 1.1.1, terá uma nova funcionalidde compátivel e uma correção de um bug ou pequena melhoria. <br/><br/>
Caso queira se aprofundar, essa foi a referência utilizada: <a href="https://www.devdofuturo.com/versionamento-semantico-o-que-e-e-como-aplicar">www.devdofuturo.com/versionamento-semantico-o-que-e-e-como-aplicar</a>
