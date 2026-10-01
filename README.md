# EC Destaque Barbershop — Agendamento (POC)

Página única (SPA) de agendamento para a barbearia **EC Destaque Barbershop** ([@ec_cortes](https://www.instagram.com/ec_cortes/)).

Mesma arquitetura dos projetos irmãos (agenda-lash / House of Beauty Care):
React 18 + Babel + Tailwind via CDN, tudo em um único `index.html` — não precisa de build.

## Visual
Identidade de barbearia: fundo preto marmorizado, dourado e prata, coroa, poste de barbeiro. Logo em `img/logo.jpeg`.

## Como rodar
Abra o `index.html` no navegador (ou publique no GitHub Pages).

## Fluxo
1. **Serviços** — lista com preços e duração.
2. **Agendamento** — nome, WhatsApp, data e horário (gerados por dia da semana).
3. **Sucesso** — envia a mensagem pronta pro WhatsApp da barbearia.

## O que configurar antes de usar de verdade
No topo do `<script>` em `index.html`, no objeto `BARBEARIA`:

- `whatsapp`: número real (formato `55` + DDD + número). Hoje é placeholder.
- `scriptGoogleUrl`: URL do Google Apps Script da agenda. Vazio = modo POC (horários simulados).
- `endereco`: endereço da barbearia (opcional, aparece na home).

Horários de funcionamento ficam no objeto `HORARIO` (por dia da semana).
Serviços e preços ficam no array `SERVICOS` — fáceis de editar.

> Os preços e horários atuais são de referência. Ajuste conforme a barbearia.
