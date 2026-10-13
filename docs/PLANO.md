# Plano de construção

Regra de ouro: o Omni-EcoRescue V3 não muda até 20/10/2026. O Nexus é separado (repositório, container e endereço próprios).

**Decisão do time:** começar pelo **funcionamento sem internet**. É o pedido do time, é a demonstração mais forte e não depende dos agentes (que precisam de internet para vigiar as fontes).

| Fase | Camadas | Entrega | Agentes |
|---|---|---|---|
| **0. Fundação** | — | Base de código copiada da V3; trocar chaves; fechar portas expostas; chip próprio do projeto | — |
| **1. Sem internet no celular** | 6 | App do cidadão offline: botão **"Baixar minha região"** (abrigos, hospitais, telefones 199/193/192, guia do que fazer, checklist, último alerta, mapa do bairro). GPS mostra distância e direção até o abrigo. Pedido de ajuda e "estou bem" ficam guardados e saem sozinhos quando o sinal volta | — |
| **2. Sem internet no abrigo** | 7 | Protótipo do **Nó Nexus**: notebook ou Raspberry + Wi-Fi local "NEXUS-ABRIGO" (quem conecta abre o app sem internet) + 2 rádios Meshtastic (abrigo fala com abrigo) + rota offline + registro de pessoas e procura de parentes | Guardião do Abrigo |
| **3. Ver e confirmar** | 2, 3 | Agente vigia + tela "Saúde das fontes" + Nota de Confiança + leitura de alertas no padrão CAP | Sentinela, Mecânico, Juiz |
| **4. Calcular e avisar** | 4, 5 | Área de impacto por evento; alerta por CEP com **SIM do operador**; registro de quem aprovou. O alerta também desce para os Nós Nexus pelo rádio | Calculista, Analista, Redator, Despachante |
| **5. Conversar** | 6 | Atendente no WhatsApp e SMS para quem não tem dados | Atendente |
| **6. Gente** | 1, 9 | Rede de voluntários; dia de simulado; reencontro de famílias; relatório pós-evento | Ouvinte, Relator |
| **7. Céu** | 8 | Ponte por Starlink; estação de satélite meteorológico (SDR) | — |

**Transversal, em todas as fases:** segurança, energia e as [Leis do Enxame](LEIS.md).

## Demonstração-alvo (ao fim da fase 2)

Desligar a internet na frente da banca e mostrar:
1. o celular continua mostrando o abrigo mais perto e o caminho (fase 1);
2. um celular sem internet conecta no Wi-Fi do abrigo e abre o app (fase 2);
3. uma mensagem sai de um abrigo e chega no outro pelo rádio LoRa (fase 2).

## Material da fase 2
- 2 rádios Meshtastic (LoRa 915 MHz, homologados para o Brasil)
- 1 notebook velho ou Raspberry Pi
- Power bank grande ou bateria com painel solar pequeno
