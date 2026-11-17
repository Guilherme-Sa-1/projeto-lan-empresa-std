# Projeto 01 — Rede LAN Empresarial

## Objetivo

Desenvolver uma simulação de infraestrutura de rede local (LAN) para uma pequena empresa, utilizando Cisco Packet Tracer.

O objetivo foi praticar a configuração de equipamentos de rede, endereçamento IPv4 e testes de conectividade entre dispositivos.

## Topologia

A infraestrutura contém:

- 1 roteador Cisco 2911
- 1 switch Cisco 2960
- 6 computadores
- 1 rede local IPv4

## Plano de endereçamento IP

| Dispositivo | Endereço IP |
|---|---|
| Roteador (Gateway) | 192.168.10.1 |
| PC-ADM-01 | 192.168.10.10 |
| PC-ADM-02 | 192.168.10.11 |
| PC-ADM-03 | 192.168.10.12 |
| PC-TI-01 | 192.168.10.20 |
| PC-TI-02 | 192.168.10.21 |
| PC-TI-03 | 192.168.10.22 |

**Máscara de sub-rede:** 255.255.255.0

**DNS configurado:** 8.8.8.8

## Configurações realizadas

- Configuração de interface GigabitEthernet no roteador.
- Configuração de endereço IPv4 estático.
- Definição do gateway padrão.
- Conexão dos computadores ao switch.
- Ativação da interface do roteador.

## Testes realizados

- `ping 192.168.10.1` — teste de conectividade entre computador e gateway.
- `arp -a` — consulta à tabela ARP.
- `ipconfig /all` — verificação das configurações de rede.

## Resultados

A comunicação entre o computador e o roteador foi estabelecida com sucesso, sem perda de pacotes no teste realizado.

Também foi identificada a associação entre o endereço IP do gateway e seu endereço MAC por meio da tabela ARP.

## Tecnologias utilizadas

- Cisco Packet Tracer
- IPv4
- Ethernet
- ARP
- ICMP
- LAN

## Arquivo do laboratório

O arquivo `empresa-lan-basica.pkt` contém a simulação desenvolvida no Cisco Packet Tracer.

## Aprendizados

Este laboratório permitiu compreender na prática os fundamentos de redes locais, endereçamento IPv4, comunicação entre dispositivos e funcionamento do protocolo ARP.