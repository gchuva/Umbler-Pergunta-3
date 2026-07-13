# Umbler-Pergunta-3

# Um cliente relata que os e-mails enviados pelo site dele estão caindo em spam ou não chegam ao
destino. Você precisa investigar e orientar o cliente (que não é técnico)

# Onde você verificaria os logs de entrega no Exim e o que procuraria?

R: tail -1000f /var/log/exim_mainlog

# Log de rejeições - e-mails bloqueados por política
tail -1000f /var/log/exim_rejectlog

# Log de emergência - erros críticos do Exim
tail -1000f /var/log/exim_paniclog

# Como você verificaria se o IP está em blacklist e o que comunicaria ao cliente em linguagem
não técnica?

Pesquisaria pelo IP do cliente junto ao orgão AntiSpam Spamhaus por exemplo.
