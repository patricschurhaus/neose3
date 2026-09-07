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
| `concorrentes/` | logotipos de concorrentes, para quadros comparativos |
| `fotos/` | fotografia de fábrica, papelão e paisagem industrial |

## Como referenciar

```html
<img src="https://raw.githubusercontent.com/patricschurhaus/neose3/main/produtos/ffg.png">
```

Use nomes de arquivo em ASCII, sem espaço e sem acento: caractere fora do ASCII
vira escape na URL e quebra em cliente de e-mail e visualizador de PDF.

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
