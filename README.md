# lab_n8n-s3-file-automation

Objetivo: n8n recebe arquivo via webhook, faz upload para S3 e notifica (Telegram/Slack).

Adicionar no n8n-s3-file-automation/README.md:

flowchart LR
    User((Usuário)) --> Webhook[n8n Webhook]
    Webhook --> S3[(AWS S3)]
    S3 --> Notify{Notificação}
    Notify --> Telegram[Telegram]
    Notify --> Slack[Slack]
