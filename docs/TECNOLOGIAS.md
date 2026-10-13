# Tecnologias

O Nexus não inventa tecnologia nova: junta o que já é usado no mundo, com o humano no comando.

## Usadas no mundo

| Tecnologia | O que é | Quem usa | No Nexus? |
|---|---|---|---|
| Cell Broadcast | A antena manda a mesma mensagem a todos os celulares da área | Brasil, Japão, Coreia, EUA, Alemanha, Holanda | Não (exclusivo de governo e operadoras) |
| SMS | Mensagem com cadastro | Brasil (40199) | Sim (fase 3+) |
| Push de app | Notificação com internet | Ucrânia, Israel, Alemanha, Coreia | Sim |
| CAP | Formato padrão internacional de alerta | EUA, Alemanha, Coreia, ONU | Sim (fase 1) |
| Satélite → alto-falantes | Alerta em segundos nas ruas | Japão, México | Alto-falante do abrigo (fase 4) |
| Rádio VHF doméstico | Receptor que toca sozinho | EUA, México | Futuro |
| Celular como sensor | Acelerômetro detecta tremor | Google Android | Relato do cidadão na Nota de Confiança |
| IA de previsão de enchente | Modelos treinados com rios do mundo | Google Flood Hub | Como fonte (fase 1) |
| Gêmeo digital da Terra | Supercomputadores simulando o planeta | Destination Earth (Europa) | Visão de longo prazo |
| LoRa / Meshtastic | Rádio de texto, longo alcance, sem internet | Comunidades e pesquisa em desastres | Sim (fase 4) |
| Mensagem por satélite | Celular fala direto com o satélite | Starlink, BeiDou, QZSS | Fase 6 |

## Escolhidas para o Nexus

| Camada | Tecnologia | Para quê |
|---|---|---|
| App offline | PWA + Service Worker | "Modo Spotify" |
| Mapa offline | OpenStreetMap em arquivo (PMTiles) | Mapa do bairro salvo no celular |
| Rota offline | OSRM local | Rota dentro do Nó Nexus |
| IA local | Ollama / llama.cpp + modelo pequeno | IA do abrigo sem nuvem |
| Agentes | openclaw + n8n | O Enxame |
| Mensagens | WAHA (WhatsApp), SMS por chip próprio | Avisar |
| Rádio | Meshtastic (LoRa, 915 MHz no Brasil) | Abrigo conversa com abrigo |
| Padrão de alerta | CAP | Conversar com a Defesa Civil |
| Satélite do clima | SDR + antena (ex.: SatDump) | Ver o clima sem internet |
| Ponte | Starlink | Cidade isolada falando com o mundo |
| Base | FastAPI + React (herdados da V3) | API e telas |
