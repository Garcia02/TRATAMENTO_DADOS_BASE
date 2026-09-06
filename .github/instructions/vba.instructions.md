# Instruções para desenvolvimento VBA

Estas instruções se aplicam aos arquivos e módulos VBA do projeto.

## Padrões de código

- Use `Option Explicit` em todos os módulos.
- Declare variáveis com o tipo mais específico possível.
- Use `Long` para índices e contagens.
- Prefira constantes e enums a valores mágicos.
- Evite estado global; quando necessário, mantenha-o encapsulado.
- Use `ThisWorkbook` e referências qualificadas em vez de objetos ativos.
- Mantenha procedimentos curtos e com uma única responsabilidade.

## Tratamento de erros

- Valide parâmetros e pré-condições antes de executar operações.
- Use um fluxo de tratamento de erros consistente.
- Não oculte erros com `On Error Resume Next`; limite seu uso a operações
  justificadas e valide imediatamente o resultado.
- Informe contexto suficiente para diagnosticar falhas.
- Restaure configurações temporariamente alteradas, como cálculo, eventos e
  atualização de tela.

## Organização

- Separe módulos de domínio, infraestrutura, utilitários e interface.
- Evite dependências circulares entre módulos.
- Mantenha nomes de procedimentos e variáveis em um idioma consistente.
- Atualize a documentação de arquitetura quando introduzir um novo componente.
