# ceinmart-ChatGPT

Estilo CSS/UserCSS para a extensão [Stylus](https://github.com/openstyles/stylus), destinado a ampliar a área de conversas e o editor de prompts do ChatGPT sem distorcer tabelas e relatórios.

**Versão inicial:** 1.0.0 — 04/11/2026, 16:56 BRT  
**Projeto:** ceinmart · Código preparado por ChatGPT (OpenAI)

## Funcionalidades

- Conversas e respostas mais largas (largura padrão: `95vw`).
- Ajuste de largura do compositor (prompt) junto com a área de respostas.
- Tabelas do componente `data-d-table-viewport` com rolagem horizontal dentro da área disponível (correção previamente validada em conversa).
- Contenção de blocos de código, imagens e conteúdo extenso.
- Ajustes de largura para páginas de relatórios do ChatGPT.
- Aplicação responsiva em telas menores, sem mudar cores e elementos de navegação.

## Instalação

1. Instale a extensão **Stylus** no Chrome.
2. Abra o arquivo [ceinmart-ChatGPT.user.css](./ceinmart-ChatGPT.user.css) pelo GitHub e selecione **Raw**, ou use o [link direto do arquivo](https://raw.githubusercontent.com/ceinmart/stylus-ceinmart-ChatGPT/main/ceinmart-ChatGPT.user.css).
3. Se o Stylus detectar o arquivo UserCSS, confirme a instalação.
4. **Desative os estilos antigos** aplicados ao ChatGPT para evitar conflitos, mantendo apenas `ceinmart-ChatGPT`.
5. Atualize a página do ChatGPT (`Ctrl+Shift+R`).

## Atualizações

O cabeçalho do arquivo inclui `@updateURL` e `@downloadURL` para permitir atualização pelo Stylus. Em versões futuras, o arquivo na branch `main` será a referência. Use a função de verificação de atualizações do Stylus. O navegador não sincroniza automaticamente todas as configurações locais da extensão.

## Configuração

Edite a declaração `--ceinmart-thread-width: 95vw` no início das regras para alterar a largura pretendida (ex.: `90vw` ou `98vw`). O valor final é limitado à largura da janela para evitar transbordamento.

## Estrutura

- `ceinmart-ChatGPT.user.css` — arquivo instalável no Stylus.
- `README.md` — documentação e notas de manutenção.

## Histórico

| Versão | Data | Alterações |
|---|---|---|
| 1.0.1 | 04/11/2026 | Largura padrão ampliada de 80vw para 95vw. |
| 1.0.0 | 04/11/2026 | Unificação do estilo pessoal v1.2.0 com a correção de tabelas validada no StretchGPT gpt.3, ajustes de editor e relatórios. |

## Limitações

O ChatGPT altera frequentemente sua estrutura HTML/CSS. Os seletores procuram priorizar atributos `data-*` e variáveis de layout, mas parte da compatibilidade depende da versão da interface. O ajuste do editor e o estilo consolidado **ainda precisam ser validados visualmente** nos seus dispositivos.

## Referências

- Base de largura: estilo pessoal fornecido pelo proprietário (v1.2.0, autor indicado como `G`).
- Correção de tabelas: adaptação realizada durante esta conversa sobre StretchGPT v7.5.2, com confirmação funcional para `data-d-table-viewport`.
