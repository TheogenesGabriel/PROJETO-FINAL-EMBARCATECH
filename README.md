# PROJETO-FINAL-EMBARCATECH
# 🌱 Sistema de Monitoramento e Controle para Rosas do Deserto

Este projeto é um sistema embarcado projetado para monitorar e controlar automaticamente as condições ideais de cultivo de Rosas do Deserto. Ele mede temperatura, umidade do solo e luminosidade, além de permitir a rega automática e manual. Também emite alertas visuais e sonoros caso os parâmetros estejam fora do ideal.

## 🚀 Funcionalidades

### 📊 Monitoramento em Tempo Real
- Medição contínua de temperatura, umidade do solo e luminosidade.
- Exibição dos dados em um display OLED 128x64.

### 💧 Rega Automática e Manual
- Acionamento automático da rega quando a umidade do solo está abaixo do ideal.
- Rega manual acionada por um botão físico.

### ⚠️ Alertas e Notificações
- Alertas sonoros e visuais (buzzer e LEDs coloridos) quando as condições estão inadequadas.
- Indicadores de saúde da planta (saudável, leve estresse, médio estresse, grave estresse).

### 🎛 Interface Simples
- Controle por botões e joystick para navegação entre as telas de informações.

### 💦 Economia de Água
- Sistema otimizado para evitar desperdício, garantindo rega eficiente e adequada às necessidades das Rosas do Deserto.

---

## 🛠 Componentes Utilizados

### 🔌 Hardware
- **Microcontrolador**: Raspberry Pi Pico
- **Display**: OLED 128x64 (I2C)
- **Sensores**:
  - Sensor de umidade do solo (ADC)
  - Sensor de temperatura (ADC)
  - Sensor de luminosidade (ADC)
- **Atuadores**:
  - Bomba de água (para rega)
  - Buzzer (para alertas sonoros)
  - LEDs (indicadores de estado: vermelho, verde e azul)
- **Controles**:
  - Botões para acionamento manual e navegação
  - Joystick para seleção de modos

---

## 🔧 Como Funciona

### 1️⃣ Inicialização
- O sistema configura os sensores, atuadores e display.
- Exibe a tela inicial com os dados coletados.

### 2️⃣ Monitoramento
- Os sensores captam os dados em intervalos programados.
- O display exibe as informações coletadas.

### 3️⃣ Controle de Rega
- Se a umidade do solo estiver abaixo de 10%, o sistema ativa a bomba automaticamente.
- O usuário pode ativar a rega manualmente pelo botão dedicado.

### 4️⃣ Alertas
- Se a umidade for muito baixa ou a luminosidade estiver fora do ideal, o sistema alerta com um som e acende LEDs vermelhos.

### 5️⃣ Navegação
- O usuário pode alternar entre diferentes telas usando o joystick.

---

## 📏 Parâmetros Ideais para Rosas do Deserto
- **Temperatura:** 20°C a 35°C
- **Umidade do Solo:** 10% a 30%
- **Luminosidade:** 50% a 70%

---

## 📜 Estrutura do Código

- **Inicialização:** Configuração dos pinos, sensores, atuadores e display.
- **Loop Principal:** Captura de dados, lógica de controle e atualização do display.
- **Funções Principais:**
  - `rega_automatica()`: Controla a rega automática.
  - `rega_manual()`: Aciona a rega manual.
  - `avaliarSaude()`: Avalia a condição da planta.
  - `play_sound()`: Emite alertas sonoros.
- **Funções de Exibição:**
  - `tela_inicial()`: Mostra os dados principais.
  - `draw_tree()`: Representa visualmente a saúde da planta.

---

## 🛠 Instalação e Uso

### 🔌 Hardware
1. Conecte os sensores, atuadores e display ao Raspberry Pi Pico conforme o esquema elétrico.
2. Certifique-se de que a bomba de água está corretamente instalada e o reservatório cheio.

### 💻 Software
1. Carregue o código no Raspberry Pi Pico usando a **Thonny IDE** ou outra ferramenta compatível.
2. Inicialize o sistema e monitore os dados exibidos no display.

### 🎮 Operação
- O sistema inicia automaticamente a leitura dos sensores e ativa a rega quando necessário.
- O usuário pode interagir via botões e joystick para alternar entre as telas de informações.

---

## 📷 Fotos do Projeto

![Imagem do WhatsApp de 2025-02-25 à(s) 18 01 51_4768c6c6](https://github.com/user-attachments/assets/79e93bd3-853e-45b7-baef-3e6e7ba9a8ce)


---

## 🎥 Vídeo Demonstrativo

(https://youtu.be/OKKcXN4V0XYo)

---


## 📆 Desenvolvedor
- **Theógenes Gabriel Aráujo de Andrade**
- **Data do Projeto:** 25/10/2023

---


Caso tenha dúvidas ou sugestões, sinta-se à vontade para contribuir! 🌵🚀

