# 🚀 Projeto Didático de IoT – Elevador com Arduino, LEGO, WPF e MQTT

Este projeto foi desenvolvido com fins **educacionais** para demonstrar aos alunos do curso técnico em Desenvolvimento de Sistemas o uso do protocolo **MQTT** aplicado à Internet das Coisas (IoT).

A solução integra:

- 🖥️ Uma aplicação **WPF (C#)** que atua como **Publisher**, recebendo dados do Arduino via porta serial e publicando em tópicos MQTT.
- 🔧 Um **Arduino** com sensores ultrassônicos e de fim de curso, simulando um **elevador didático**.
- 📡 Um **Subscriber (WPF)** que consome as mensagens MQTT e exibe em interface gráfica.
- ☁️ O broker MQTT utilizado foi o público [test.mosquitto.org](https://test.mosquitto.org/).

---

## 🎯 Objetivos Didáticos

- Mostrar na prática como funciona a comunicação **Publisher → Broker → Subscriber** no MQTT.  
- Ensinar conceitos de **QoS (Quality of Service)** no protocolo.  
- Integrar hardware (Arduino) e software (WPF) em um projeto funcional.  
- Fornecer aos alunos uma experiência aplicada de **IoT**.

---

## ⚙️ Tecnologias Utilizadas

- **Arduino UNO**  
- **Sensores ultrassônicos e HW-870** para detecção de altura e limites do elevador  
- **C# WPF** para as interfaces gráficas (Publisher e Subscriber)  
- **MQTTnet** (biblioteca MQTT para .NET)  
- **Broker público test.mosquitto.org**

---

## 🏗️ Arquitetura da Solução

```mermaid
flowchart LR
    A[Arduino com sensores] -- Serial --> B[Aplicação WPF Publisher]
    B -- MQTT --> C[(Broker MQTT)]
    C -- MQTT --> D[Aplicação WPF Subscriber]

```

## 📸 Demonstração

### 🔹 Hardware: controle subida e descida
![Foto do Elevador](https://github.com/FredOnBrasil/Elevador_LEGO_IoT_MQTT/blob/main/Imagens/Controle_de_subida_e_descida_elevador.jpg)

### 🔹 Hardware: lateral do elevador
![Foto lateral](https://github.com/FredOnBrasil/Elevador_LEGO_IoT_MQTT/blob/main/Imagens/Lateral_elevador.jpg)

### 🔹 Hardware: vista superior
![Foto vista superior](https://github.com/FredOnBrasil/Elevador_LEGO_IoT_MQTT/blob/main/Imagens/Vista_superior.jpg)

### 🔹 Hardware: placa parte posterior
![Foto vista posterior](https://github.com/FredOnBrasil/Elevador_LEGO_IoT_MQTT/blob/main/Imagens/Montagem_parte_posterior.jpg)

### 🔹 Hardware: vista lateral
![Foto vista lateral](https://github.com/FredOnBrasil/Elevador_LEGO_IoT_MQTT/blob/main/Imagens/Lateral_elevador.jpg)

### 🔹 Hardware: vista frontal
![Foto vista frontal](https://github.com/FredOnBrasil/Elevador_LEGO_IoT_MQTT/blob/main/Imagens/vista_frontal.jpg)

### 🔹 Interface Publisher (WPF)
![Publisher](https://github.com/FredOnBrasil/Elevador_LEGO_IoT_MQTT/blob/main/Imagens/Interface_publisher.png)

### 🔹 Interface Subscriber (WPF)
![Subscriber](https://github.com/FredOnBrasil/Elevador_LEGO_IoT_MQTT/blob/main/Imagens/interface_subscriber.png)

### 🔹 Interface Publisher/Subscriber (WPF)
![Pub_Sub1](https://github.com/FredOnBrasil/Elevador_LEGO_IoT_MQTT/blob/main/Imagens/publisher_e_subscriber_3.png)

### 🔹 Interface Publisher/Subscriber (WPF)
![Pub_Sub3](https://github.com/FredOnBrasil/Elevador_LEGO_IoT_MQTT/blob/main/Imagens/publisher_subscriber.png)
