Investigação do Analista SOC 
Após recebimento do alerta Phishing no SIEM, o objetivo do Analista SOC é verificar se a mensagem representa uma tentativa real de comprometimento e identificar possiveis impactos no ambiente. 

O que chamou a atenção ?
A investigação inicia com identificação dos principais indicadores que justificam a abertura de alerta. Entre eles, destacam-se:
- Login realizado em horario incomum para o usuario 
- Tentativas de Autenticação a partir de um endereço IP desconhecido 
- Alerta gerado pelo gateway de e-mail indicando possivel phishing 
Esses eventos indicam a necessidade de aprofundar a investigação para confirmar ou descartar um comprometimento.

Quais evidencias devem ser analisadas ?
Com o alerta identificado, o proximo passo é coletar evidencias que permitam validar o incidente.
- Cabeçalho do E-mail: Verificar o remetente 
- URL recebida: Analisar se o endereço direciona para um dominio legitimo ou pagina criada para roubo de credenciais (Sandbox)
- Endereço IP Origem: Identificar a localização, reputação e possiveis atividades maliciosas associadas ao IP (Whois)
- Logs do SIEM: correlacionar eventos de autenticação, acessos e demais alertas relacionados ao usuário ou ao ativo comprometido.
- Logs do EDR: verificar a execução de arquivos suspeitos, criação de processos, conexões externas e demais comportamentos incomuns no endpoint.
- Histórico de autenticação: comparar os acessos recentes com o padrão de utilização do usuário, identificando logins fora do horário habitual, dispositivos desconhecidos ou localidades incomuns.
Ao reunir essas evidências, o Analista SOC consegue confirmar se houve comprometimento, avaliar o impacto do incidente e definir as ações de contenção e resposta mais adequadas.

Conclusão
A análise de um ataque de phishing vai além da identificação de um e-mail malicioso. O trabalho do Analista SOC consiste em reunir evidências, correlacionar eventos e compreender o comportamento do atacante para confirmar o incidente e reduzir seus impactos.

Neste estudo de caso, foi possível observar como um simples clique em um link fraudulento pode resultar no comprometimento de credenciais e, consequentemente, no acesso não autorizado aos sistemas da organização. O uso do MITRE ATT&CK auxiliou no mapeamento das etapas do ataque, fornecendo uma referência para compreender as técnicas utilizadas pelo adversário e orientar a investigação.

Esse processo demonstra a importância da análise de logs, da validação de indicadores de comprometimento (IOCs) e da adoção de medidas de contenção, reforçando o papel do Analista SOC na identificação, investigação e resposta a incidentes de segurança.
