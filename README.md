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
| `produtos/` | os produtos de papelão ondulado |
| `bandeiras/` | bandeiras de estado |
| `marca/` | logotipo Irani |
| `concorrentes/` | logotipos de concorrentes, para quadros comparativos |
| `fotos/` | fotografia de fábrica, papelão e paisagem industrial |

## Como referenciar

```html
<img src="https://raw.githubusercontent.com/patricschurhaus/neose3/main/produtos/maleta.png">
```

Use nomes de arquivo em ASCII, sem espaço e sem acento: caractere fora do ASCII
vira escape na URL e quebra em cliente de e-mail e visualizador de PDF.
