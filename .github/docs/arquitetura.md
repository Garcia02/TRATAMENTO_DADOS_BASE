# Arquitetura do projeto

## Objetivo

Este documento descreve as decisões estruturais do projeto VBA e deve ser
atualizado quando novos componentes ou fluxos relevantes forem adicionados.

## Organização proposta

Os componentes VBA devem ser organizados por responsabilidade:

- **Domínio**: regras de negócio e validações.
- **Infraestrutura**: leitura e escrita em planilhas, arquivos e integrações.
- **Utilitários**: funções reutilizáveis sem regra de negócio específica.
- **Interface**: formulários, eventos de planilha e rotinas acionadas pelo
  usuário.

## Fluxo recomendado

1. A interface recebe a solicitação do usuário.
2. O domínio valida e processa os dados.
3. A infraestrutura persiste ou consulta os dados.
4. A interface apresenta o resultado ou uma mensagem de erro contextualizada.

## Princípios

- Baixo acoplamento entre componentes.
- Responsabilidade única por procedimento e módulo.
- Referências explícitas a objetos do Excel.
- Tratamento de erros próximo da operação que pode falhar.
- Documentação das decisões que afetem manutenção ou compatibilidade.
