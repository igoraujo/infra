# Tabalho de infra

### Trabalho deve ser feito individualmente ou em duplas.
A ENTREGA DEVE SER FEITA VIA CLASSROOM ATÉ ÀS 23:59 DO DIA 02 DE JUNHO (enviar o arquivo .PKT com o nome
dos integrantes). **Trabalhos entregues após essa data, cópias totais ou parciais, além de configurações feitas parcial ou integralmente sem a aplicação de comandos (salvo quando necessário) não serão avaliados.**


## CRIAÇÃO DO CENÁRIO:


A empresa *"ABC"* possui um escritório em Belo Horizonte e acessa serviços de servidores em um datacenter de Madri. O projeto de rede que deve ser implementado está descrito abaixo:

------

_Em Belo Horizonte a empresa ocupa um prédio de 8 andares. A distribuição dos setores pelos andares é feita da seguinte maneira:_

**TÉRREO*: Recepção
**1º ANDAR:** Departamento Pessoal | RH
**2º ANDAR:** Comercial | Projetos
**3º ANDAR:** Financeiro | Contabilidade
**4º ANDAR:** Compras | Jurídico
**5º ANDAR:** TI | Logística
**6º ANDAR:** Diretoria
**7º ANDAR:** Datacenter

------

_As redes em Belo Horizonte são separadas por VLANs:_

**VLAN 10:** Servidores (192.168.10.0 /26)
**VLAN 20:** Diretoria (192.168.20.0 /28)
**VLAN 30:** Rede Corporativa (172.30.0.0 /21)
**VLAN 40:** Rede Visitantes (10.40.0.0 /18)

------

__Servidores:__


**INTRANET:** 192.168.10.10
**DNS:** 192.168.10.20 (configurar serviço)
**HTTP:** 192.168.10.30 (configurar serviço)
**ARQUIVOS:** 192.168.10.40


------


__Desktops:__

Deve haver pelo menos **3 computadores** por departamento, todos devem receber IPs via **DHCP**


------


__Serviços em Madri:__

**EMAIL:** 172.10.10.100 /28
**BD:** 172.10.10.150 /28
**APLICAÇÃO:** 172.10.10.200 /28


------


__Outras informações__

**WAN:** 201.30.20.0/30
**REDE BH:** Protocolo **OSPF**
**REDE MADRI:** Roteamento **estático**

## REGRAS E RESTRIÇÕES:


------


Todas as redes devem se comunicar, exceto a VLAN 40 que deve ser isolada da rede corporativa.


## REQUISITOS OBRIGATÓRIOS


1. Deve haver um switch principal no datacenter (Esse switch deve ser o VTP Server);
1. Deve haver no mínimo 1 switch por andar (todos configurados como VTP Client);
1. Deve haver roteamento entre as VLANS 10, 20 e 30.
1. **A rede de visitantes deve ser distribuída por wireless.**


## OBSERVAÇÕES E INFORMAÇÕES ADICIONAIS


- Serão avaliadas as configurações de cada computador, as configurações de cada switch e de suas VLANs, as
configurações dos roteadores e a organização das redes (a disposição dos elementos na tela e suas respectivas
identificações) no Cisco Packet Tracer. Portanto, lembre-se de dar nomes e descrição aos dispositivos da rede.
- Qualquer informação como IPs, equipamentos, senhas e etc. que não tenham sido citados neste documento e que sejam
fundamentais na construção do seu projeto, você deve incluir e documentar no seu trabalho.
- Você é livre para criar alternativas para que o seu trabalho funcione.
