# GitLab

Pra renomear a branch padrão:

1. Na barra lateral vá para "Repository" > "Branches".

2. Clique em "New branch".

3. Escreva o novo nome da branch padrão, tenha certeza que a branch padrão atual está selecionada em "Create from" e confirme.

4. Na barra lateral vá para "Settings" > "Repository".

5. Na seção "Default branch" selecione a nova branch padrão e salve.

6. Na seção "Protected branches" proteja a nova branch padrão com as mesmas configurações usadas com a anterior.

Isso deve renomear a branch padrão mas não irá atualizar os merge requests apontados para essa branch.

Você precisa atualizar cada merge request para a nova branch ou fazer isso com algum script usando a API.

Seu repositório será alterado apenas no servidor, então após isso continue com o guia para renomear todas as cópias locais.
