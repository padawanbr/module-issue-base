<!--- Preencha as informações abaixo para criar uma nova issue --->

## Título da issue

<!--- Descrição detalhada da issue --->

## Solução proposta

<!--- Descreva como você planeja resolver a issue --->

<!--- Trecho de código para acionar a action e criar o pull request --->

<!---
- name: Criar Pull Request
  uses: peter-evans/create-pull-request@v3.11.0
  with:
    base: nome_da_branch_de_destino
    head: ${{ github.event.issue.user.login }}:nome_da_branch_de_origem
    title: ${{ github.event.issue.title }}
    body: ${{ github.event.issue.body }}
--->
