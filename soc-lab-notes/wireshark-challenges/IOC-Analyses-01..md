Laboratorio SOC- Investigacao de um IOC utilizando Wireshark

Ojetivo
Simular uma investigaçao de um indicador de comprometimento (IOC) utilizando o Wireshark para analisar comunicaçoes de rede

Cenario
Durante uma analise de trafego foi identificado o endereço 13.227.207.111. O objetivo foi investigar a comunicaçao estabelecida entre o cliente e esse servidor

Metodologia
- Captura de pacotes na interface Wi-Fi
- Aplicaçao do Filtro: 
Ip.addr == 13.227.207.111
- Analise dos protocolos DNS, TCP e TLS
- Verificaçao do estabelecimento da conexao HTTPS

Evidencias encontradas
- O cliente iniciou a comunicaçao a partir do endereco IP local
- A conexao utilizou a porta 443 (HTTPS) 
- Foi observado o TCP -Three Way Handshake
- Foram identificados o TLS Client Hello e o TLS Server Hello, indicando a negociaçao de uma sessao criptografada

Arquivos da Captura
As capturas utilizadas nesta analise estao disponiveis neste diretorio:
- Wireshark DNS.pcapng
- Wireshark TLS.pcapng
- Wireshark flags.pcapng

Conclusao
A analise demonstrou o fluxo completo de uma conexao HTTPS, desde a resolução de nommes ate o estabelecimento da comunicaçao criptografada. Esse tipo de investigaçao é immportante para atividades de Threat Hunting e analise inicial de incidentes e ambientes SOC.

Competencias Praticas
- Analise de Trafego de Rede
- Investigaçao de IOC
- DNS
- TCP Three-Way Handshake
- TLS Handshake
- Wireshark
