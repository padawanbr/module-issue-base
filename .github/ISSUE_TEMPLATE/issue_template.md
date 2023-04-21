name: Auto PR

on:
  issues:
    types: [opened]

jobs:
  auto_pr:
    runs-on: ubuntu-latest
    steps:
    - name: Checkout
      uses: actions/checkout@v3
    - name: Create PR
      uses: peter-evans/create-pull-request@v5
      with:
    base: nome_da_branch_de_destino
    head: nome_da_branch_de_origem
        commit-message: "Auto PR: Fixes #${{ github.event.issue.number }}"
        title: "Auto PR: Fixes #${{ github.event.issue.number }}"
        body: "This PR was automatically generated to resolve issue #${{ github.event.issue.number }}."
