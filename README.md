Dispositivo Inteligente de Gerenciamento de Energia Elétrica⚡️

Este projeto foi desenvolvido como trabalho de conclusão de curso para a obtenção do título de Técnico em Eletrónica e Telecomunicações no Instituto Politécnico da Humpata (Lubango, 2025).
[...](imagens/video1.GIF)
* ![Video da montagem](imagens/IMG-20250804-WA0013.jpg)

O objetivo principal foi criar um dispositivo eletrónico eficiente, seguro e acessível para o gerenciamento inteligente e monitoramento do consumo de energia elétrica em ambientes residenciais, visando mitigar o desperdício e combater a inadimplência.

---

## ⚙️ Diferencial do Projeto vs. Sistemas Atuais
Os medidores eletrónicos pré-pagos convencionais são instalados no interior das residências, exigindo o carregamento manual de créditos e alertando o usuário localmente. 
O nosso dispositivo foi projetado para ser implementado **diretamente nos postes de distribuição de energia**, gerenciando de forma centralizada e simultânea o consumo de até 5 residências. A interação e o carregamento de crédito são feitos de forma totalmente remota através de uma aplicação móvel dedicada.

---

## 🛠️ Arquitetura do Sistema

### 1. Hardware e Eletrónica (Sistemas Embarcados)
O protótipo físico foi estruturado com foco em precisão de leitura e segurança de rede:
* **Processamento:** Microcontroladores (Família Arduino/ESP32) gerenciando a lógica do sistema.
* **Sensores de Medição:** Utilização de sensores de corrente alternada (SCT-013) e sensores de tensão instalados no circuito para monitoramento em tempo real.
* **Atuação:** Módulos de relés para interrupção e restabelecimento automático do fornecimento elétrico com base no saldo disponível.
* **Comunicação:** Tecnologia sem fios de longo alcance (LoRa) para a transmissão estável de dados entre o poste e a central.

### 2. Software e Integração Mobile (IoT)
A aplicação móvel desenvolvida apresenta duas interfaces totalmente distintas:
* **Interface do Usuário:** Monitoramento de consumo instantâneo (dados de saldo em Kwanzas e volume em kWh), histórico gráfico semanal, canais de emergência e recargas facilitadas via métodos de pagamento integrados (cartão de débito/Multicaixa Express).
* **Interface do Administrador (Distribuidora):** Dashboard central para monitoramento do status da rede em tempo real, monitoramento de falhas ativas, envio de notificações urgentes e gestão/ajuste de tarifas de mercado.

### 3. Sistema de Segurança Ativa e Antifraude
Para prevenir perdas comerciais e vandalismo, o sistema integra barreiras físicas e digitais:
* **Deteção de Intrusão:** Alarme sonoro dedicado acionado por sensores físicos (tipo *reed switch*) em caso de abertura forçada da caixa selada do dispositivo.
* **Deteção de Desvios:** Alerta automático enviado via rede LoRa ou aplicação para o administrador em caso de cortes ou desvios de corrente não autorizados.
* **Proteção Elétrica:** Conjunto de disjuntores integrados para proteger os sensores sensíveis contra sobrecargas e curtos-circuitos.
---
**Equipa de Autores:** Ericleny Lende, Gabriel Garcia, João Catengue, Magno Daniel e Paulina Mulumbi.  
**Tutora:** Joana Chalale.