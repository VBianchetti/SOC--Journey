O MITRE ATT&CK é um framework amplamente utilizado na área de Cibersegurança que documenta as táticas, técnicas e procedimentos (TTPs) utilizados por adversários durante ataques cibernéticos. Ele serve como referência para compreender o comportamento dos atacantes e apoiar atividades de detecção, investigação e resposta a incidentes.

Como funciona ?
Ele é organizado de forma simples para identificar os momentos de um ataque. 
Taticas (Tatics) - Objetivo do atacante - Exemplo: Coleta de Credenciais, Movimento Lateral
Tecnicas (Techniques) - Metodo especifico (Como) - Exemplo: Phishing via Email, Exploração de serviço RDP 
Subtécnicas (Sub-Techniques) - detalham variações ou forma especifica 

Como Analista SOC utiliza o MITRE ATTACK ?
Quando um alerta é gerado por um SIEM ou EDR, o Analista SOC pode relacioná-lo a uma técnica do MITRE ATT&CK, como T1566.001 – Spearphishing Attachment. Esse mapeamento padroniza a classificação dos incidentes, facilita a comunicação entre equipes e fornece contexto para a investigação e resposta ao ataque.

Adiante teremos um estudo de caso: Ataque Phishing 
Um colaborador recebe um E-mail informando que sua senha expirou e precisa ser redefinida. Sem analisar quem enviou aquele e-mail, ele clica no link que direciona a um site malicioso que se assemelha ao sistema que a empresa usa. Após inserir suas credencias, o atacante obtem acesso a conta 
