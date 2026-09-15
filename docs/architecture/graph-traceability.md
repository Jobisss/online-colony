# Graph Traceability

O projeto mantém um grafo de rastreabilidade em `graphify-out/`. Ele conecta conceitos, políticas, interações e decisões aos documentos e seções onde aparecem.

## Pré-requisito

O pacote **Graphify precisa estar instalado** no ambiente antes de continuar. Sem ele, não execute consultas nem considere a atualização concluída. Verifique a instalação com:

```powershell
python -c "import graphify; print('Graphify instalado')"
```

Se a verificação falhar, instale o pacote antes de prosseguir:

```powershell
python -m pip install graphifyy
```

Depois confirme novamente o import e só então execute o fluxo de atualização.

## Fluxo para mudanças

Antes de alterar um conceito transversal, consulte o grafo pelo nome do conceito. Para Fauna, por exemplo:

```powershell
python -m graphify query "Fauna" --budget 1200 --graph graphify-out/graph.json
python -m graphify affected "Regional Fauna" --depth 2 --graph graphify-out/graph.json
```

Use os nós retornados como checklist de impacto: abra cada arquivo e seção indicada, confirme se a mudança também afeta políticas, interações, pesquisa, combate, produção, autonomia ou economia, e atualize os documentos correspondentes.

Depois de modificar documentação, regenere o grafo incrementalmente:

```text
/graphify E:\jobisss\online-colony --update
```

O processo deve atualizar `graph.json`, `graph.html` e `GRAPH_REPORT.md`. Relações `EXTRACTED` vêm de referências explícitas; `INFERRED` são dependências prováveis e devem ser revisadas; `AMBIGUOUS` exige decisão manual.

## Artefatos

- `graphify-out/graph.html`: exploração visual interativa, sem servidor.
- `graphify-out/graph.json`: dados consultáveis e fonte da visualização.
- `graphify-out/GRAPH_REPORT.md`: comunidades, nós centrais e conexões surpreendentes.

O grafo é um índice de impacto, não substitui a revisão do texto. Quando uma mudança for aceita, mantenha as referências de seção atualizadas para que a próxima consulta continue encontrando o impacto correto.
