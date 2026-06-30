O Que é o MITRE ATTACK ? 
Um Framework globalmente reconhecido de ameaças ciberneticas que fornece um conhecimento detalhado das táticas e técnicas que adversários usam durante um ataque cibernetico

Como funciona ?
Ele é organizado de forma simples para identificar os momentos de um ataque. 
Taticas - Objetivo Macro (Porquê do Ataque) - Exemplo: Coleta de Credenciais, Movimento Lateral
Tecnicas - Metodo especifico (Como) - Exemplo: Phishing via Email, Exploração de serviço RDP 
Procedimento - Implementações reais especificas - Exemplo: Mimikatz, Cobalt Srike

Como Analista SOC utiliza o MITRE ATTACK ?
Quando chega um alerta no SIEM ou EDR o analista pode usar o MITRE como uma técnica de identificação, por exemplo (T1566.001 - Spearphishing Attachment), assim padroniza os Tickets e elimina ambiguidade nas escaladas. 

Adiante teremos um estudo de caso: Ataque Phishing 
Um colaborador recebe um E-mail informando que sua senha expirou e precisa ser redefinida. Sem analisar quem enviou aquele e-mail, ele clica no link que direciona a um site malicioso que se assemelha ao sistema que a empresa usa. Após inserir suas credencias, o atacante obtem acesso a conta 
