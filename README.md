# guia-completo-git-github
Formação Github Certification

🚀 Guia Completo de Git e GitHub

Do zero ao fluxo profissional de colaboração

📌 O que é Git?

O Git é um sistema de controle de versão distribuído criado por Linus Torvalds em 2005.

Ele permite que desenvolvedores:

Salvem versões do código ao longo do tempo

Trabalhem em equipe sem sobrescrever o trabalho uns dos outros

Voltem para versões anteriores se algo der errado

Criem ramificações (branches) para testar novas funcionalidades

Diferente de salvar arquivos como:

projeto_final_agora_vai.zip
projeto_final_agora_vai_versao2.zip

O Git organiza tudo de forma estruturada e rastreável.

🧠 Conceitos Fundamentais do Git
📂 Repositório (Repository)

É onde o projeto fica armazenado e versionado.

Pode ser:

Local → na sua máquina

Remoto → hospedado em plataformas como o GitHub

🗂 Working Directory

É a pasta do seu projeto onde você faz alterações.

📌 Staging Area (Index)

Área intermediária onde você prepara as alterações antes de confirmar (commit).

💾 Commit

É o registro de uma alteração no histórico do projeto.

Cada commit possui:

Um identificador único (hash)

Autor

Data

Mensagem explicativa

Exemplo:

git commit -m "Adiciona funcionalidade de login"
🔁 Fluxo Básico do Git
git init              # Inicia um repositório
git status            # Mostra o estado atual
git add .             # Adiciona arquivos à staging area
git commit -m "msg"   # Cria um commit

Fluxo visual:

Working Directory → Staging Area → Commit
🌳 Branches (Ramificações)

Uma branch é uma linha paralela de desenvolvimento.

Por padrão, temos a branch:

main

Criando uma nova branch:

git checkout -b nova-feature

Voltando para main:

git checkout main

Mesclando:

git merge nova-feature

Branches permitem trabalhar em novas funcionalidades sem afetar o código principal.

🔀 Merge e Conflitos

Quando duas pessoas alteram a mesma parte do código, pode ocorrer um conflito de merge.

O Git mostrará algo assim:

<<<<<<< HEAD
Seu código
=======
Código da outra pessoa
>>>>>>> branch

Você deve decidir qual versão manter (ou combinar ambas), depois:

git add .
git commit -m "Resolve conflito"
🌍 O que é GitHub?

O GitHub é uma plataforma que hospeda repositórios Git na nuvem.

Ele permite:

Colaboração em equipe

Controle de acesso

Pull Requests

Issues

Integração com CI/CD

Versionamento online

🔗 Conectando Git ao GitHub

Adicionar repositório remoto:

git remote add origin https://github.com/usuario/repositorio.git

Enviar alterações:

git push origin main

Clonar um repositório:

git clone https://github.com/usuario/repositorio.git
🔁 Trabalhando em Equipe

Fluxo comum em times profissionais:

Criar uma branch

Fazer alterações

Commitar

Dar push

Abrir Pull Request

Revisão de código

Merge

📌 Pull Request (PR)

Um Pull Request é um pedido para que suas alterações sejam analisadas e incorporadas à branch principal.

Permite:

Revisão de código

Discussões

Aprovação

Histórico organizado

🐛 Issues

Issues servem para:

Reportar bugs

Sugerir melhorias

Organizar tarefas

Documentar problemas

📜 Arquivo .gitignore

Arquivo que define o que NÃO deve ser versionado.

Exemplo:

node_modules/
.env
bin/
obj/
⚙️ Comandos Intermediários Importantes
Ver histórico:
git log
Ver diferenças:
git diff
Alterar último commit:
git commit --amend
Reverter commit:
git revert <hash>
Reset (cuidado!):
git reset --hard <hash>
🏗 Fluxos de Trabalho Profissionais
🔵 Git Flow

Branches principais:

main

develop

feature/*

release/*

hotfix/*

Muito usado em projetos grandes.

🟢 GitHub Flow

Mais simples:

main sempre estável

Cada funcionalidade em uma branch

Pull Request para integrar

Muito usado em startups e times ágeis.

🔐 Boas Práticas

✔ Commits pequenos e frequentes
✔ Mensagens claras
✔ Uma responsabilidade por commit
✔ Nunca commitar arquivos sensíveis
✔ Sempre atualizar sua branch antes de dar merge

🎯 Conclusão

Git não é apenas uma ferramenta, é uma forma de pensar desenvolvimento.

Ele permite:

Organização

Segurança

Colaboração

Escalabilidade

Aprender Git é um divisor de águas para qualquer desenvolvedor.
