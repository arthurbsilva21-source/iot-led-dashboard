# Central de Iluminação IoT

Dashboard IoT de altíssimo nível estético, moderno e minimalista para controle de um LED na porta 13 do Arduino via MQTT.

## 🎨 Características

- ✨ Design Glassmorphism premium com gradiente azul-branco
- 📱 Totalmente responsivo (Mobile, Tablet, Desktop)
- 🔗 Conexão MQTT automática via HiveMQ Broker (SSL)
- 💡 LED virtual com efeito neon pulsante
- 🎛️ Botões intuitivos LIGAR/DESLIGAR
- 🔴🟡🟢 Status de rede em tempo real
- 📝 Input dinâmico para gerenciar tópicos MQTT

## 🚀 Acesso Rápido

[**Abra o Dashboard →**](https://arthurbsilva21-source.github.io/iot-led-dashboard/)

## 📋 Configuração

**Tópico MQTT Padrão:** `gerry_sanchez_led_exclusivo/arduino`

**Broker:** broker.hivemq.com:8884 (WebSockets Seguro)

**Comandos:**
- Publica `1` para **LIGAR** o LED
- Publica `0` para **DESLIGAR** o LED

## 🔧 Arquitetura

- Biblioteca Paho MQTT via CDN
- ClientID gerado dinamicamente
- Callback `onMessageArrived()` garante sincronismo
- LED muda apenas quando mensagem retorna do broker

## 📚 Ideal para

- Aulas de IoT e Arduino
- Projetos educacionais com MQTT
- Demonstração de arquitetura Publisher/Subscriber
