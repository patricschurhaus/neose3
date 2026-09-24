# neose3 — assets públicos

Imagens usadas nos materiais web da **Plataforma Neos**, da Irani Papel e Embalagem.

O repositório é público, e as páginas consomem as imagens direto daqui por `<img src>`.

## Regra única

**Só entra conteúdo público.**

Nada de dado financeiro, estudo de mercado, documento interno, planilha,
apresentação, especificação de fornecedor ou material de marca não divulgado.
Este repositório existe para hospedar fotografia e logotipo — nada mais.

O `.gitignore` bloqueia formatos de documento de propósito. Se um arquivo seu
não está sendo versionado, provavelmente é isso, e provavelmente está certo.

## Organização

| pasta | o que guarda |
|---|---|
| `produtos/` | os produtos de papelão ondulado, **um arquivo por código do `codelist`** do simulador |
| `bandeiras/` | bandeiras de estado |
| `marca/` | logotipo Irani |
| `logos/` | logotipos de empresas do setor, **um arquivo por código de empresa** da base `PET-01` |
| `fotos/` | fotografia de fábrica, papelão e paisagem industrial |

## Como referenciar

```html
<img src="https://raw.githubusercontent.com/patricschurhaus/neose3/main/produtos/ffg.png">
```

Use nomes de arquivo em ASCII, sem espaço e sem acento: caractere fora do ASCII
vira escape na URL e quebra em cliente de e-mail e visualizador de PDF.

## `logos/` usa o código de três letras da empresa

Mesmo princípio dos produtos: **o nome do arquivo é a chave**, não o nome
comercial. O código é o `emp` da aba `empresas` da base do setor — `KLA`,
`MIT`, `BHS` — em maiúsculas, sempre `.png`.

```
logos/KLA.png    logos/MIT.png    logos/BHS.png
```

Assim nenhuma página precisa de tabela de-para: ela monta a URL a partir do
código que já tem em mãos. Logo nova aparece sozinha nas páginas já publicadas,
sem reempacotar nada — basta subir o arquivo com o nome certo.

**Sempre `.png`.** A extensão faz parte do contrato: a página adivinha a URL e
não tem como descobrir que um arquivo é `.svg`. Se você tem o vetor, guarde-o
onde quiser e exporte um `.png` para cá.

Se o arquivo não existir, a página desenha um bloco com a sigla — **falta de
logo nunca vira buraco na tela.** Não há pressa em completar.

## Os quatro produtos usam o código do simulador

O nome do arquivo é o **código do objeto** na aba `codelist` do simulador, não o
nome comercial. Assim a imagem, a cor do produto no site e a variável da
planilha se chamam a mesma coisa, e não existe tabela de-para para envelhecer.

| arquivo | código | produto |
|---|---|---|
| `produtos/ffg.png` | `ffg` | caixa maleta — casemaker (*flexo folder gluer*) |
| `produtos/rdc.png` | `rdc` | caixa de corte e vinco — *rotary die cutter* |
| `produtos/shm.png` | `shm` | chapa para mercado |
| `produtos/acs.png` | `acs` | acessórios |

Trocar a arte de um produto é substituir o arquivo mantendo o nome: as páginas
apontam para cá e recarregam sozinhas.
