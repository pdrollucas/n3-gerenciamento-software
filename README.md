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
