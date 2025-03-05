name: Relatar um Problema
description: Use este template para reportar um problema ou bug encontrado.
title: "[BUG] Descreva brevemente o problema"
labels: [bug, triagem]
assignees: ""

body:
  - type: textarea
    id: descricao_problema
    attributes:
      label: "Descrição do problema"
      description: "Descreva o problema encontrado com detalhes."
      placeholder: "O que aconteceu? Como reproduzir? O que era esperado?"
    validations:
      required: true

  - type: textarea
    id: referencias
    attributes:
      label: "Referências"
      description: "Adicione links, documentos, prints ou qualquer material relevante."
      placeholder: "Exemplo: Logs, prints, links para outras issues, documentação relacionada."

  - type: dropdown
    id: prioridade
    attributes:
      label: "Prioridade"
      description: "Qual a urgência desse problema?"
      options:
        - Baixa
        - Média
        - Alta
    validations:
      required: true

  - type: textarea
    id: pessoas_envolvidas
    attributes:
      label: "Pessoas envolvidas"
      description: "Mencione as pessoas envolvidas (@usuario)."
      placeholder: "@usuario1, @usuario2, ..."

  - type: textarea
    id: issues_relacionadas
    attributes:
      label: "Issues relacionadas"
      description: "Se houver, mencione issues relacionadas ao problema."
      placeholder: "Exemplo: #123, #456"
