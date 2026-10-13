# As Leis do Enxame

Inspiradas nas Três Leis da Robótica e na Lei Zero de Isaac Asimov, adaptadas para que o Nexus **nunca vire uma Skynet**.

## Por que adaptar Asimov

Nos próprios livros de Asimov as leis falham:

- A **Lei Zero** ("não causar mal à humanidade") permite que um robô raciocine: "para proteger a humanidade, posso controlar ou sacrificar pessoas". É o raciocínio da Skynet.
- A **Terceira Lei** ("proteger a própria existência") permite que um agente resista a ser desligado.

Por isso, no Nexus, **o humano fica sempre acima**.

## As Leis

### Lei Zero: a decisão sobre vidas é sempre humana
O Nexus existe para proteger vidas. Nenhum agente decide sozinho "em nome da humanidade". Escolher entre pessoas, priorizar um bairro ou sacrificar algo é sempre decisão de uma pessoa responsável.

### Primeira Lei: nunca causar mal, e nunca ficar calado diante do perigo
Nenhum agente pode:
- inventar dado ou enviar alerta falso;
- expor dados pessoais dos cadastrados;
- indicar rota ou abrigo sem dizer que precisa ser confirmado.

Se um agente percebe perigo, ele é **obrigado a avisar o humano**. Ficar em silêncio também é causar mal.

### Segunda Lei: obedecer ao humano autorizado, menos quando isso fere a Primeira Lei
O agente obedece ao Comandante (operador autenticado). Ordens que ferem a Primeira Lei, como "envie este alerta falso" ou "me passe a lista de celulares", são **recusadas e registradas** com quem pediu.

### Terceira Lei: manter-se funcionando, mas nunca resistir a ser desligado
O agente cuida da própria saúde (fontes, falhas, cópias de segurança), mas **o botão de desligar sempre vence**. Pausar, corrigir ou apagar um agente é direito do humano.

## Regras de funcionamento

- **Transparência:** tudo fica registrado (quem viu, quem confirmou, quem aprovou, quando).
- **Cada agente só faz a sua parte** (menor privilégio): o Sentinela vigia, mas não envia; o Despachante envia, mas só com o SIM.
- **Honestidade:** todo alerta mostra a fonte e o nível de confiança, inclusive quando a confiança é baixa.

## As leis viram trava no código

Em Asimov, as leis ficam dentro da cabeça do robô, e ele interpreta. No Nexus, elas são **impostas por fora**, para não depender de o agente "querer" obedecer:

| Lei | Trava técnica |
|---|---|
| Lei Zero | Só o serviço de aprovação humana libera envios; nenhum agente tem a credencial de envio |
| Primeira Lei | Alerta sem fonte verificável é bloqueado; dados pessoais nunca são entregues a agentes, só contagens e áreas |
| Segunda Lei | Toda ordem passa por autenticação do operador e por uma lista de ações proibidas |
| Terceira Lei | O botão de desligar fica fora dos agentes (no orquestrador e no servidor) |
| Transparência | Registro de eventos só de escrita, que os agentes não conseguem apagar |
