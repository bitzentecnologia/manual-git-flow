Manual de Git e Git-Flow 
=======================================================
> Manual de Boas Práticas para o uso do Git e Git-Flow em projetos realizados pelas equipes da Bitzen.

## 🔎 O que é?

Git-Flow é uma estratégia de branching para Git que ajuda a simplificar o gerenciamento de publicações e correções, isolando o código em tipos diferentes de branches.

## 🧭 Fluxo

Existem 5 tipos de branches diferentes que complementam o fluxo da ferramenta:
- 🟢 **Main** - Faixa de Produção
  - _Nota: A branch "main" também pode ser nomeada como "master"._
  - O propósito da branch "main" é conter todo código pronto para produção, revisado e que pode ser lançado.  
- 🚧 **Develop** - Faixa de Homologação
  - A branch "develop" é criada no início do projeto e mantida ao decorrer do processo de desenvolvimento do software. 
  - Seu propósito é conter código pré-produção com novas funcionalidades que estão em processo de teste.
- 💡 **Feature** - Criação de funcionalidades
  - A branch "feature" é a mais comum no fluxo do Git-Flow. É usada para adicionar novas funcionalidades ao código. 
  - Quando criada, ela se baseia no estado atual da branch "develop" 
  - Ao finalizar, é feito o merge automaticamente com a branch "develop" e a branch "feature" é deletada.
- 🚀 **Release** - Lançamento de versão em Produção
  - A branch "release" deve ser usada apenas em preparação para novas publicações em produção. Ela é baseada no estado atual da "develop".
  - Tipicamente, ela conterá código de toques finais e correções menores especificamente para o código em lançamento.
  - Também é gerada uma tag única contendo a versão do software. A tag deve ser enviada ao repositório para controle de releases. 
- 🚒 **Hotfix** - Apagar incêndios em Produção
  - A branch "hotfix" é usada para atacar rapidamente mudanças necessárias na branch "main".
  - Seu propósito é conter código com prioridade alta o suficiente para burlar a relase e ir direto para produção. Exemplo: Mudanças emergenciais, breaking-bugs em produção.

Tópicos<a name="content"></a>
-------------
- [Desenvolvimentos e Melhorias: Features](features.md)
- [Correções de bugs: Bugfixes](features.md)
- [Publicações em produção: Releases](features.md)
- [Correções de bugs em produção: Hotfixes](features.md)
- [Pull Requests: Como e quando usar?](features.md)
- [Organização e manutenção do repositório](features.md)

## 🤝 Colaboradores

Agradecemos às seguintes pessoas que contribuíram para este manual:

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/renan-bitzen">
        <img src="https://avatars.githubusercontent.com/u/88667733?v=4" width="100px;"/><br>
        <sub>
          <b>Renan Lima</b>
        </sub>
      </a>
    </td>
  </tr>
</table>