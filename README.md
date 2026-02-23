# Redirecionamento DP — Central de Atendimento

Uma página estática para direcionamento de chamados e portais clientes, criada para facilitar o encaminhamento de solicitações de Departamento Pessoal (DP), RH e demais canais.

Demo (Hospedagem): https://alldax-contabilidade.github.io/redirecionamento_dp/

**Tecnologias:** HTML5, Tailwind CSS, JavaScript

## Visão geral

Esta aplicação é uma landing page simples que centraliza links para portais de atendimento (RH, folha de pagamento e demais canais). Inclui suporte para upload de logo via uma integração de SDK (`elementSdk`) e permite configuração dinâmica de título, nome da empresa e URLs dos portais.

## Demonstração ao vivo

O site está publicado no GitHub Pages e pode ser acessado em:

- https://alldax-contabilidade.github.io/redirecionamento_dp/

## Recursos

- Links direcionados para portais de RH e portal geral.
- Upload de logo do cliente (via `elementSdk`).
- Layout responsivo construído com Tailwind CSS.
- Código simples, fácil de customizar e reaproveitar.

## Como executar localmente

Opções rápidas:

- Abrir diretamente o arquivo `index.html` no navegador.
- Servir via um servidor HTTP simples (recomendado para recursos locais e testes):

PowerShell / Terminal:

```powershell
python -m http.server 8000
# então abra http://localhost:8000 no navegador
```

## Estrutura do projeto

- `index.html` — página principal com todo o markup, estilos e scripts.
- `README.md` — documentação do projeto.

## Configuração e personalização

- O projeto injeta um SDK (`/_sdk/element_sdk.js`) que expõe `window.elementSdk` para configurar dinamicamente:
	- `company_name`, `welcome_title`, `link_rh_url`, `link_outros_url`, `logo_data`.
- Para personalizar o texto e os links em ambiente integrado, utilize a API `elementSdk.init()` conforme exemplificado em `index.html`.

## Contribuindo

- Sugestões, correções e melhorias são bem-vindas via pull request.
- Abra uma issue descrevendo o objetivo antes de iniciar mudanças maiores.

## Licença

Nenhuma licença foi especificada neste repositório.

## Contato

Para dúvidas ou suporte, entre em contato com o mantenedor do repositório.

