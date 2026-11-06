# CadastroEE — Estácio, Mundo 3, Nível 4

Sistema cadastral web acadêmico com Servlets, JSP, JPA e EJB, desenvolvido no Apache NetBeans.

**Integrante indicado no projeto:** Lucas Alves.

## Objetivos da atividade

- Persistência de dados com JPA.
- Regras de negócio em EJBs.
- Exibição e entrada de dados com Servlets e JSPs.
- Interface com Bootstrap.

## Organização

| Caminho | Finalidade |
| --- | --- |
| `build.xml` e `nbproject/` | Projeto agregador Ant/NetBeans `CadastroEE` |
| `CadastroEE-ejb/` | Módulo de negócio e persistência |
| `CadastroEE-war/` | Módulo web |
| `CadastroEE-war/web/` | Páginas como `ProdutoLista.jsp` e `ProdutoDados.jsp` |

As propriedades do projeto declaram nível de fonte/alvo **Java 11**, plataforma **9.1** e tipo de servidor GlassFish `gfv610ee9`. O pacote agregado é `CadastroEE.ear`.

## Preparar e executar

```sh
git clone https://github.com/alvesvslucas/Miss-o-Pratica-Nivel-4-Mundo-3.git
cd Miss-o-Pratica-Nivel-4-Mundo-3
```

1. Abra a pasta raiz como projeto no Apache NetBeans.
2. Cadastre um servidor GlassFish compatível com a plataforma configurada e selecione um JDK aceito por esse servidor; o nível Java 11 dos fontes não define sozinho o JDK do servidor.
3. Confirme que os módulos `CadastroEE-ejb` e `CadastroEE-war` são reconhecidos.
4. Prepare o banco de teste, driver JDBC e recurso de persistência exigidos pelo módulo EJB, usando configurações locais.
5. Use **Limpar e Construir** no projeto agregado e depois **Executar** para implantação pelo NetBeans.

## Estado

A configuração completa de banco, driver e servidor precisa ser confirmada antes de reproduzir a aplicação. O esquema do banco e o datasource devem corresponder à configuração do módulo EJB. Compilação, implantação do EAR e operações cadastrais não foram executadas nesta revisão.
