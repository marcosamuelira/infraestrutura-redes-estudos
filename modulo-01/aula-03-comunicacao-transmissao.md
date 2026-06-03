# Aula 03 -  Comunicação e Transmissão em Redes, Analógico, Digital e Tipos e Métodos

## 🎯 Objetivo da Aula

Compreender como os dados são convertidos, transmitidos e entregues em uma rede de computadores, além dos principais tipos de comunicação utilizados na infraestrutura de redes.

---

## Conversão Analógico e Digital (ADC e DAC)

Os computadores trabalham apenas com informações digitais (0 e 1). Por isso, muitas informações precisam ser convertidas durante o processo de comunicação.

## ADC (Analog to Digital Converter)

### O que é?

Converte sinais analógicos em sinais digitais.

### Exemplo

🎤 Ao falar em um microfone:

* Sua voz é analógica.
* O microfone converte para digital.
* O computador processa os dados.

### Frase para decorar

✅ ADC = Humano → Computador

---

## DAC (Digital to Analog Converter)

### O que é?

Converte sinais digitais em sinais analógicos.

### Exemplo

🔊 Ao ouvir um áudio:

* O computador envia dados digitais.
* A caixa de som converte para analógico.
* Você escuta o som.

### Frase para decorar

✅ DAC = Computador → Humano

📡 Meios de
 Transmissão

## ⚡ Sinais Elétricos (Par Metálico)

### O que é?

Utilizam corrente elétrica para transmitir dados.

### Características

* Baixo custo.
* Sofrem interferência eletromagnética.

### Exemplo

Cabos de rede de cobre (UTP).

---

## 💡 Sinais de Luz (Fibra Óptica)

### O que é?

Utilizam pulsos de luz para transmitir dados.

### Características

* Alta velocidade.
* Não sofrem interferência eletromagnética.
* Exigem cuidado com curvas excessivas.

### Exemplo

Internet de fibra óptica residencial.

---

## 📶 Micro-ondas e Rádio Frequência

### O que é?

Utilizam ondas eletromagnéticas sem fio para transmitir dados.

### Características

* Permitem mobilidade.
* Podem sofrer interferências.

### Exemplos

* Wi-Fi
* 4G
* 5G
* Rádio
* TV

---

# 🔢 Transmissão Digital

## O que é?

Os computadores trabalham utilizando apenas dois estados:

* 0 = ausência de sinal
* 1 = presença de sinal

Toda informação transmitida pela rede é convertida para sequências de bits.

### Exemplo

Uma foto, vídeo ou mensagem do WhatsApp é transformada em milhares de bits antes de ser enviada pela rede.

### Resumo

Tudo que trafega na rede é convertido em 0 e 1.

---

# 📦 Métodos de Transmissão

## Paralela

### O que é?

Transmite vários bits simultaneamente utilizando múltiplos canais.

### Vantagens

* Alta velocidade em curtas distâncias.

### Desvantagens

* Os sinais podem chegar em momentos diferentes.
* Sofre mais interferências.
* Pouco utilizada em redes modernas.

### Exemplo

Imagine 8 corredores largando ao mesmo tempo em pistas diferentes.

Mesmo saindo juntos, alguns podem correr mais rápido e chegar antes dos outros.

Na transmissão paralela acontece algo parecido: os bits são enviados simultaneamente, mas podem chegar em tempos diferentes ao destino.

### Resumo

✅ Vários bits ao mesmo tempo.
❌ Maior risco de sincronização incorreta.

---

## Serial

### O que é?

Transmite um bit por vez através de um único canal.

### Vantagens

* Mais confiável.
* Melhor para longas distâncias.
* Menor interferência.
* Método mais utilizado atualmente.

### Exemplo

Imagine uma fila de pessoas entrando em um ônibus.

Cada pessoa entra uma de cada vez, mantendo a ordem correta.

Na transmissão serial os bits também seguem uma sequência organizada até o destino.

### Resumo

✅ Um bit por vez.
✅ Mais confiável para redes modernas.

---

# 🔄 Comunicação Síncrona e Assíncrona

## Comunicação Síncrona

### O que é?

Os dispositivos trabalham sincronizados por um mesmo ritmo de transmissão.

### Exemplo

Uma banda tocando seguindo um metrônomo.

Todos os músicos precisam acompanhar o mesmo ritmo.

### Exemplos de tecnologias

* SDSL
* HDSL

---

## Comunicação Assíncrona

### O que é?

Cada dispositivo transmite quando necessário, sem sincronização constante.

### Exemplo

Uma conversa no WhatsApp.

Você envia uma mensagem agora e recebe resposta depois.

### Exemplo de tecnologia

* ADSL

---

# 🔁 Tipos de Comunicação

## Simplex

### O que é?

A comunicação ocorre em apenas uma direção.

### Exemplos

📺 TV

📻 Rádio

Você recebe a informação, mas não responde.

---

## Half Duplex

### O que é?

Os dois lados podem transmitir, mas não ao mesmo tempo.

### Exemplos

📟 Walkie-talkie

📞 Nextel

Um fala enquanto o outro escuta.

---

## Full Duplex

### O que é?

Os dois lados transmitem e recebem simultaneamente.

### Exemplos

📱 Ligação telefônica

🌐 Redes cabeadas modernas

Você fala e escuta ao mesmo tempo.

---

# 📦 Encapsulamento e Desencapsulamento

## Encapsulamento

### O que é?

Processo de adicionar informações de controle aos dados para que possam viajar pela rede.

### Exemplo

📦 Envio pelos Correios:

1. O produto é colocado na caixa.
2. É adicionada uma etiqueta.
3. É informado o endereço.
4. É gerado um código de rastreamento.

Na rede ocorre algo semelhante: cada camada adiciona informações necessárias para a entrega correta dos dados.

---

## Desencapsulamento

### O que é?

Processo de remover as informações adicionadas durante o transporte.

### Exemplo

📦 Quando a encomenda chega:

1. A etiqueta já cumpriu sua função.
2. A caixa é aberta.
3. As embalagens são removidas.
4. O produto é entregue ao destinatário.

Na rede, cada camada remove suas informações até que os dados cheguem à aplicação.

---

# 🚦 Segmentação de Dados

## O que é?

Grandes quantidades de dados são divididas em partes menores para facilitar o transporte.

### Exemplo

🚚 Mudança residencial.

É mais fácil transportar várias caixas pequenas do que uma única caixa gigante.

### Benefícios

* Melhor controle.
* Maior eficiência.
* Possibilidade de reenviar apenas a parte perdida.

---

# 🚗 Multiplexação

## O que é?

Técnica que permite que vários dados utilizem o mesmo meio de transmissão simultaneamente.

### Exemplo

Imagine uma rodovia com várias faixas.

Nela circulam:

* Carros
* Caminhões
* Ônibus
* Ambulâncias

Todos utilizam a mesma estrada ao mesmo tempo, mas cada um segue para um destino diferente.

Na rede acontece a mesma coisa:

* E-mails
* Vídeos
* Navegação web
* Chamadas VoIP

Todos compartilham o mesmo meio físico de transmissão.

### Resumo

✅ Vários fluxos de dados.
✅ Mesmo meio de transmissão.

---

# 📨 Tipos de Comunicação em Rede

## Unicast

### O que é?

Um remetente envia dados para um único destinatário.

### Exemplo

Mensagem privada no WhatsApp.

Pessoa A ➜ Pessoa B

---

## Broadcast

### O que é?

Um remetente envia dados para todos os dispositivos da rede.

### Exemplo

Síndico anunciando algo pelo alto-falante do condomínio.

Todos recebem a mensagem.

---

## Multicast

### O que é?

Um remetente envia dados para um grupo específico de dispositivos.

### Exemplo

Reunião no Teams com participantes selecionados.

Somente os membros do grupo recebem os dados.

---

## Anycast

### O que é?

Os dados são enviados para o servidor disponível mais próximo ou mais eficiente.

### Exemplo

A Netflix possui servidores em:

* São Paulo
* Rio de Janeiro
* Curitiba
* Brasília

Quando você acessa um filme em São Paulo, normalmente será atendido pelo servidor mais próximo ou pela melhor rota disponível.

Já um usuário em Curitiba poderá ser atendido por outro servidor.

O conteúdo é o mesmo, mas cada usuário utiliza um servidor diferente.

### Exemplos Reais

* Netflix
* Cloudflare
* Servidores DNS públicos

### Resumo

✅ Mesmo serviço.
✅ Servidores diferentes.
✅ Atendimento pelo servidor mais próximo ou mais eficiente.

---

# 🌐 IPv4

## Identificadores de Rede

Cada dispositivo conectado à rede possui identificadores para ser encontrado.

### Endereço IP

* Identifica o dispositivo na rede.
* Pode mudar conforme a rede utilizada.

### Endereço MAC

* Identifica fisicamente a placa de rede.
* É único para cada dispositivo.

### Exemplo

🏢 Condomínio:

* IP = Número do apartamento.
* MAC = CPF do morador.

O apartamento pode mudar, mas o CPF continua sendo o mesmo.

### Frase para Decorar

✅ IP = Identifica a localização na rede.
✅ MAC = Identifica fisicamente o dispositivo.

---

# 🧠 Resumo para Memorizar

* ADC = Analógico → Digital
* DAC = Digital → Analógico
* Fibra óptica utiliza luz.
* Cabos de cobre utilizam sinais elétricos.
* Serial é o método mais utilizado atualmente.
* Full Duplex permite enviar e receber simultaneamente.
* Encapsulamento adiciona informações de controle.
* Desencapsulamento remove essas informações.
* Multiplexação permite vários fluxos no mesmo meio.
* Unicast = um para um.
* Broadcast = um para todos.
* Multicast = um para grupo.
* Anycast = um para o servidor mais próximo.
* IP identifica a localização do dispositivo.
* MAC identifica fisicamente o equipamento.

