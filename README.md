# 👾 Space Invaders com Arduino + LCD I2C

Projeto de um mini **Space Invaders** rodando em Arduino com tela LCD 16x2 via I2C e botões físicos.

---

## 🧰 Requisitos

Para rodar no hardware real você vai precisar de:

* 1x Arduino (Uno, Nano, etc.)
* 1x Display LCD 16x2 com módulo I2C
* 3x Botões
* Jumpers (fios)
* Protoboard (opcional)

---

## 🔌 Ligações

### 📺 LCD I2C

| LCD | Arduino |
| --- | ------- |
| VCC | 5V      |
| GND | GND     |
| SDA | A4      |
| SCL | A5      |

---

### 🎮 Botões

| Função | Pino |
| ------ | ---- |
| Mover  | 2    |
| Atirar | 3    |
| Pause  | 4    |

👉 Importante: os botões usam `INPUT_PULLUP`, então ligue:

* Um lado no pino
* Outro no **GND**

---

## 💻 Como rodar no Arduino IDE

1. Abra a **Arduino IDE**

2. Instale a biblioteca:

   * `LiquidCrystal I2C`

3. Copie e cole o código no editor

4. Conecte o Arduino no PC

5. Selecione:

   * **Placa correta**
   * **Porta COM correta**

6. Clique em **Upload**

✅ Pronto! O jogo já vai rodar na tela

---

## ▶️ Como jogar

* Botão 2 → alterna posição (cima/baixo)
* Botão 3 → atira
* Botão 4 → iniciar / pausar

---

## 🌐 Rodar sem Arduino (Simulador)

Se você não tiver os componentes, dá pra rodar online usando o:

👉 https://wokwi.com

### Passo a passo:

1. Acesse o site

2. Clique em **"New Project"**

3. Escolha **Arduino Uno**

4. Adicione:

   * LCD 16x2 I2C
   * 3 botões

5. Faça as mesmas conexões:

   * LCD → A4 (SDA), A5 (SCL)
   * Botões → pinos 2, 3 e 4

6. Cole o código no editor

7. (obrigatório) Instale a biblioteca `LiquidCrystal I2C`

8. Clique em **Start Simulation**

🎮 O jogo vai rodar direto no navegador

---

## 🧠 Observações

* O jogo tem níveis progressivos
* A velocidade aumenta conforme você avança
* O score é acumulativo
* Sistema de pause e restart incluído

---

## 🚀 Divirta-se!

Projeto simples, mas ótimo pra treinar:

* Arduino
* Lógica de jogos
* Manipulação de display LCD
