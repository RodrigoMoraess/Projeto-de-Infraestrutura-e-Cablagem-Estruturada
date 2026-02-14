# Projeto de Infraestrutura e Cablagem Estruturada

Este repositório apresenta o projeto de design e simulação de uma rede corporativa para uma empresa de médio porte, desenvolvido no **Cisco Packet Tracer**. O foco do projeto é a organização física (planta baixa) e a segmentação lógica de alta eficiência.

## 📍 Visão Geral
A rede foi projetada para suportar múltiplos departamentos isolados, garantindo segurança e uma gestão de tráfego otimizada através de sub-redes.

## 🚀 Tecnologias e Conceitos Aplicados
- **Topologia:** Estrela Estendida com infraestrutura centralizada na Sala de Redes.
- **Segmentação:** VLSM (Variable Length Subnet Masking) com máscaras `/28` para máxima eficiência de endereçamento.
- **Hardware:** Switches Cisco 2960, Roteadores, Servidores e APs Wireless.
- **Design:** Planeamento de cablagem estruturada sobre planta baixa.

## 📊 Plano de Endereçamento (VLSM)
Com base na documentação técnica do projeto, a rede está dividida nos seguintes segmentos:

| Departamento | Rede | Gateway | Máscara |
| :--- | :--- | :--- | :--- |
| **Administração** | 192.168.10.0/28 | 192.168.10.254 | 255.255.255.240 |
| **Financeiro / RH** | 192.168.20.0/28 | 192.168.20.254 | 255.255.255.240 |
| **Marketing** | 192.168.30.0/28 | 192.168.30.254 | 255.255.255.240 |
| **Serviços e Entregas**| 192.168.40.0/28 | 192.168.40.254 | 255.255.255.240 |
| **Área Técnica** | 192.168.50.0/28 | 192.168.50.254 | 255.255.255.240 |

## 🖼️ Topologia e Planta da Rede
![Topologia da Rede](screenshot/infrastructure_diagram.png)

## ⚙️ Configurações de Serviços Centrais

Para além da conectividade básica, foram implementados serviços críticos para o funcionamento da empresa:

### 🌐 Rede Wireless (Mobilidade)
- **Wireless Router:** Configurado como ponto de acesso para dispositivos móveis (Laptops e Smartphones).
- **Segurança:** Implementação de WPA2-PSK para proteção da rede Wi-Fi.
- **Isolamento:** A rede wireless está integrada no segmento de gestão para permitir mobilidade administrativa sem comprometer a segurança dos departamentos críticos.

---
*Projeto desenvolvido para portfólio de Infraestrutura de Redes e Sistemas.*
