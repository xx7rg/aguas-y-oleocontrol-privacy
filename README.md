<div align="center">

<img src="assets/x7rg-enterprise.png" alt="x7rG ENTERPRISE" width="240" />

# Política de Privacidade — Aguas y Oleocontrol

<img src="assets/aguas-y-oleocontrol.png" alt="Aguas y Oleocontrol" width="520" />

**Documento público que explica, em espanhol, como o aplicativo profissional de gestão de piscinas utiliza e protege informações.**

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-online-15d5ae?logo=github&logoColor=white)](https://xx7rg.github.io/aguas-y-oleocontrol-privacy/)
[![Validação](https://github.com/xx7rg/aguas-y-oleocontrol-privacy/actions/workflows/validate.yml/badge.svg)](https://github.com/xx7rg/aguas-y-oleocontrol-privacy/actions/workflows/validate.yml)
[![Idioma](https://img.shields.io/badge/idioma-es--ES-7c3aed)](index.html)
[![HTML](https://img.shields.io/badge/HTML5-documento-E34F26?logo=html5&logoColor=white)](index.html)

</div>

## Documento publicado

**Política online:** [xx7rg.github.io/aguas-y-oleocontrol-privacy](https://xx7rg.github.io/aguas-y-oleocontrol-privacy/)

A página apresenta as categorias de dados, finalidades, permissões do dispositivo, fornecedores, conservação, segurança e meios para exercer direitos. O conteúdo foi comparado com as funções implementadas no aplicativo **Aguas y Oleocontrol**.

## O que a política cobre

| Área | Informação documentada |
| --- | --- |
| Conta | nome, usuário, e-mail, função e permissões |
| Operação | piscinas, endereços informados, visitas, medições, tarefas e incidentes |
| Mídia | fotografias, vídeos e áudio presente em gravações de vídeo |
| Notificações | token de push, plataforma e estado de entrega |
| Segurança | sessões, auditoria, sincronização e cache temporário |
| Direitos | acesso, correção, exclusão, oposição, limitação e portabilidade, quando aplicáveis |

## Fluxo das informações

```mermaid
flowchart LR
    U[Usuário autorizado] --> A[Aplicativo]
    A --> D[Dados operacionais]
    A --> M[Fotos e vídeos opcionais]
    A --> N[Token de notificação opcional]
    D --> S[Supabase]
    M --> S
    N --> E[Expo e serviços da plataforma]
    S --> P[Equipe autorizada conforme função]
    A --> R[Relatório escolhido pelo usuário]
    R --> C[Aplicativo de e-mail ou compartilhamento]
```

## Decisões de privacidade documentadas

- o aplicativo não solicita localização GPS precisa;
- câmera, galeria, microfone e notificações dependem da permissão do usuário;
- fotografias e vídeos são usados como documentação operacional;
- não há venda de dados nem uso para publicidade comportamental declarado;
- Supabase, Expo, Apple e Google são identificados conforme sua função;
- solicitações podem ser enviadas para `contato.rgsantos@gmail.com`.

## Estrutura

```text
aguas-y-oleocontrol-privacy/
├── assets/
│   ├── aguas-y-oleocontrol.png
│   └── x7rg-enterprise.png
├── index.html
├── politica_privacidad_aguas_y_oleocontrol_es.html
├── scripts/
│   └── validate_static.py
└── README.md
```

O arquivo `index.html` é a versão vigente. O endereço antigo é mantido para compatibilidade com links já distribuídos.

## Visualizar localmente

Requisito: Python 3.

```bash
git clone https://github.com/xx7rg/aguas-y-oleocontrol-privacy.git
cd aguas-y-oleocontrol-privacy
python -m http.server 8000 --bind 127.0.0.1
```

Abra [http://127.0.0.1:8000](http://127.0.0.1:8000) e encerre o servidor com `Ctrl+C`.

### Validar arquivos e links locais

```bash
python scripts/validate_static.py
```

## Publicação

O workflow `Deploy GitHub Pages` valida e publica os arquivos estáticos após cada envio para a branch `main`. Para atualizar o documento, altere `index.html`, execute a validação local e envie a mudança ao repositório.

## Manutenção do conteúdo

A política deve ser revista sempre que o aplicativo passar a coletar outra categoria de dados, solicitar nova permissão, integrar um novo fornecedor ou alterar o processo de exclusão. O texto público deve continuar refletindo o comportamento efetivo do aplicativo.

---

<div align="center">

© 2026 **x7rG ENTERPRISE™** — Todos os direitos reservados.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rgds)
&nbsp;
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=flat&logo=instagram&logoColor=white)](https://www.instagram.com/_7ragnar/)

</div>
