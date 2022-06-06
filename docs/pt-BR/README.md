Renomear a branch padrão de seu repositório Git tanto no servidor quanto local.

# Instruções

1. Verifique todas as dependências que podem quebrar se o nome da branch padrão for alterado, como fluxos de CI/CD, integrações internas e externas, automações, documentações. Para ajudar quando for realmente alterado tente:

    - Mudar previamente os usos do nome da branch para uma variável.
    - Escrever tudo que você precisa fazer depois de renomear.
    - Comunicar todas as pessoas o que será renomeado e quando.

2. Renomeie a branch padrão no seu servidor Git remoto.

    - [GitHub](GitHub.md)
    - [GitLab](GitLab.md)

3. Rode esse script no diretório de cada clone local do reposítório. Avise as outras pessoas para fazer o mesmo.

        curl -fsSL https://raw.githubusercontent.com/ResultadosDigitais/rename_default_branch/main/rename_default_branch | bash

# Configurações

Se você não está renomeando de `master` para `main`, ajuste para os valores desejados:

    curl -fsSL https://raw.githubusercontent.com/ResultadosDigitais/rename_default_branch/main/rename_default_branch | FROM=branch-anterior TO=branch-nova bash

Opções:

- `REMOTE`: Nome do Git remote
- `FROM`: Nome da branch padrão atual
- `TO`: Novo nome da branch padrão
