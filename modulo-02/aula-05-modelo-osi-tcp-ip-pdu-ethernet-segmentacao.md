# Aula 05 - Modelo OSI, TCP/IP, PDU, Ethernet, Encapsulamento e Segmentação


## Objetivo da Aula

Compreender como os dados trafegam na rede através dos modelos OSI e TCP/IP, além dos conceitos de PDU, encapsulamento, segmentação, Ethernet e principais ataques em cada camada.

---

# Modelo OSI (Open Systems Interconnection)

## O que é?

O Modelo OSI é um modelo teórico criado para padronizar a comunicação entre dispositivos de rede.

Ele divide a comunicação em 7 camadas, permitindo entender exatamente o papel de cada etapa durante a transmissão dos dados.

### Analogia

🏢 Imagine um prédio empresarial.

Cada andar possui uma função específica:

* Recepção
* Administrativo
* Financeiro
* Jurídico
* Diretoria

Nenhum setor executa a função do outro.

No modelo OSI acontece a mesma coisa.

Cada camada possui responsabilidades específicas.

### Frase para decorar

✅ Modelo OSI = divisão da comunicação em 7 camadas.

---

# Camada 1 - Física (Physical)

## O que é?

Responsável pela transmissão dos sinais elétricos, ópticos ou sem fio.

É a camada onde os bits trafegam fisicamente.

### Exemplos

* Cabo UTP
* Fibra óptica
* Cabo coaxial
* Conectores RJ-45
* Sinais Wi-Fi

### Observação

Switches, roteadores e firewalls são equipamentos físicos, porém sua principal atuação ocorre em camadas superiores.

### Analogia

🛣️ Estrada

A estrada não escolhe o destino dos carros.

Ela apenas permite que eles trafeguem.

A camada física faz a mesma coisa com os bits.

### Frase para decorar

✅ Camada Física = transporte físico dos sinais.

---

# Camada 2 - Enlace de Dados (Data Link)

## O que é?

Responsável pela comunicação dentro da rede local.

Trabalha com endereços MAC e quadros (Frames).

### Protocolos

* Ethernet
* VLAN
* PPP
* HDLC

### Informações importantes

* Endereço MAC
* Controle de acesso ao meio
* Comunicação local

### Analogia

🏢 Condomínio

Antes de entregar uma encomenda o porteiro verifica:

* Torre
* Apartamento

Na rede a camada de enlace verifica:

* MAC de origem
* MAC de destino

### Frase para decorar

✅ Camada de Enlace = responsável pelo endereço MAC.

---

# Camada 3 - Rede (Network)

## O que é?

Responsável pelo endereçamento lógico e roteamento dos dados.

Define o caminho que os pacotes irão percorrer até chegar ao destino.

### Protocolos

* IPv4
* IPv6
* ICMP
* IPsec
* ARP

### Analogia

🗺️ GPS

O GPS determina a rota para chegar ao destino.

A camada de rede faz exatamente isso com os pacotes.

### Frase para decorar

✅ Camada de Rede = responsável pelos endereços IP.

---

# Camada 4 - Transporte (Transport)

## O que é?

Responsável por transportar os dados entre origem e destino.

Também realiza a segmentação dos dados.

### Protocolos

* TCP
* UDP
* SCTP

---

## TCP

### Características

* Orientado à conexão
* Possui confirmação de entrega
* Mais confiável

### Analogia

📦 Correios com rastreamento

O pacote é enviado.

O sistema verifica:

* Saiu?
* Chegou?
* Foi entregue?

Se necessário ocorre reenvio.

### Frase para decorar

✅ TCP = confiabilidade.

---

## UDP

### Características

* Não orientado à conexão
* Não confirma recebimento
* Mais rápido

### Analogia

📻 Rádio ao vivo

Se uma palavra for perdida durante a transmissão ela não será enviada novamente.

A transmissão continua normalmente.

### Frase para decorar

✅ UDP = velocidade.

---

# Camada 5 - Sessão (Session)

## O que é?

Responsável por criar, manter e encerrar sessões de comunicação.

### Protocolos

* SIP
* RTP

### Analogia

🎥 Reunião no Teams

A camada de sessão:

* Cria a reunião
* Mantém a reunião ativa
* Finaliza a reunião

### Frase para decorar

✅ Sessão = controla a conversa.

---

# Camada 6 - Apresentação (Presentation)

## O que é?

Responsável por preparar os dados para a aplicação.

### Funções

* Criptografia
* Descriptografia
* Compressão
* Conversão de formatos

### Protocolos

* SSL
* TLS

### Analogia

🌎 Tradutor

Converte informações para que ambas as partes possam entender.

### Frase para decorar

✅ Apresentação = tradução e proteção dos dados.

---

# Camada 7 - Aplicação (Application)

## O que é?

Camada onde ficam os programas utilizados pelos usuários.

### Exemplos

* Navegador Web
* WhatsApp
* Outlook
* Teams

### Analogia

📱 Aplicativos do celular

São os programas que o usuário realmente utiliza.

### Frase para decorar

✅ Aplicação = interface entre usuário e rede.

---

# Principais Ciberataques

## Sniffing

### O que é?

Captura de informações que trafegam pela rede.

### Analogia

👂 Escutar a conversa da mesa ao lado em um restaurante.

---

## Spoofing

### O que é?

Falsificação de identidade digital.

Pode envolver MAC, IP ou DNS.

### Analogia

🪪 Utilizar documento falso para se passar por outra pessoa.

---

## Man-in-the-Middle

### O que é?

Ataque onde o invasor fica entre origem e destino.

### Analogia

📨 Interceptar uma carta, ler o conteúdo e depois encaminhá-la ao destinatário.

---

## DoS (Denial of Service)

### O que é?

Sobrecarregar um serviço até que ele pare de responder.

### Analogia

☎️ Milhares de pessoas ligando ao mesmo tempo para um único telefone.

---

## Session Hijacking

### O que é?

Sequestrar uma sessão já autenticada.

### Analogia

🎫 Roubar o ingresso de alguém que já entrou no evento.

---

## Phishing

### O que é?

Enganar usuários para roubar informações.

### Analogia

🎣 Site falso do banco pedindo senha e dados pessoais.

---

## Exploit

### O que é?

Exploração de vulnerabilidades em aplicações.

### Analogia

🔓 Encontrar uma fechadura defeituosa e utilizá-la para entrar em uma casa.

---

# Modelo TCP/IP (Transmission Control Protocol / Internet Protocol)

## O que é?

O Modelo TCP/IP é o modelo utilizado na Internet e na maioria das redes atuais.

Diferente do Modelo OSI, que possui 7 camadas, o TCP/IP possui apenas 4 camadas.

Seu objetivo é simplificar a comunicação entre dispositivos e permitir que redes diferentes consigam trocar informações.

### Analogia

📦 Empresa de entregas

Imagine uma transportadora que possui apenas 4 departamentos:

* Atendimento
* Preparação das encomendas
* Transporte
* Entrega

Cada departamento possui uma função específica até que a encomenda chegue ao cliente.

O Modelo TCP/IP funciona da mesma forma.

### Frase para decorar

✅ TCP/IP = modelo prático utilizado na Internet.

---

# Camada de Aplicação (Application)

## O que é?

Responsável pela comunicação entre o usuário e a rede.

Ela reúne as funções das camadas:

* Aplicação
* Apresentação
* Sessão

do Modelo OSI.

### Funções

* Interface com o usuário
* Criptografia
* Compressão
* Controle de sessões
* Serviços de rede

### Protocolos

* HTTP
* HTTPS
* DNS
* FTP
* SMTP
* POP3
* IMAP

### Exemplos

* Navegador Web
* WhatsApp
* Outlook
* Teams

### Analogia

📱 Aplicativos do celular

São os programas que você utiliza diariamente para acessar serviços na rede.

### Frase para decorar

✅ Aplicação = tudo que o usuário enxerga e utiliza.

---

# Camada de Transporte (Transport)

## O que é?

Responsável pelo transporte dos dados entre origem e destino.

Também realiza a segmentação dos dados.

### Protocolos

* TCP
* UDP
* SCTP

### Funções

* Controle da comunicação
* Segmentação dos dados
* Controle de erros
* Confirmação de entrega (TCP)

### Analogia

📦 Transportadora

Recebe uma carga grande e divide em várias caixas menores para facilitar a entrega.

### Frase para decorar

✅ Transporte = entrega dos dados.

---

# Camada de Internet (Internet)

## O que é?

Responsável pelo endereçamento lógico e roteamento dos dados.

Define o caminho que os pacotes irão seguir pela rede.

### Protocolos

* IPv4
* IPv6
* ICMP
* IPsec
* ARP

### Funções

* Endereço IP de origem
* Endereço IP de destino
* Roteamento

### Analogia

🗺️ GPS

Determina qual caminho deve ser utilizado para chegar ao destino.

### Frase para decorar

✅ Internet = responsável pelos endereços IP.

---

# Camada de Acesso à Rede (Network Access)

## O que é?

Responsável pela comunicação física e local da rede.

Ela reúne as funções das camadas:

* Enlace
* Física

do Modelo OSI.

### Protocolos e Tecnologias

* Ethernet
* Wi-Fi
* PPP
* HDLC

### Funções

* Endereçamento MAC
* Transmissão dos sinais
* Comunicação local

### Analogia

🚚 Entrega final

É o momento em que a encomenda sai do caminhão e chega fisicamente ao endereço do destinatário.

### Frase para decorar

✅ Acesso à Rede = MAC, cabos e transmissão física.

---

# Comparação OSI x TCP/IP

| Modelo OSI   | Modelo TCP/IP |
| ------------ | ------------- |
| Aplicação    | Aplicação     |
| Apresentação | Aplicação     |
| Sessão       | Aplicação     |
| Transporte   | Transporte    |
| Rede         | Internet      |
| Enlace       | Acesso à Rede |
| Física       | Acesso à Rede |

---

# Resumo para Memorizar

✅ TCP/IP possui 4 camadas.

✅ Aplicação reúne Aplicação + Apresentação + Sessão do OSI.

✅ Transporte continua responsável pelo TCP e UDP.

✅ Internet trabalha com IP e roteamento.

✅ Acesso à Rede reúne Enlace + Física.

✅ O Modelo TCP/IP é o modelo utilizado na Internet atualmente.

# PDU (Protocol Data Unit)

## O que é?

PDU (Protocol Data Unit) é o nome dado às unidades de dados que trafegam pela rede.

Conforme os dados passam pelas camadas dos modelos OSI e TCP/IP, eles recebem nomes diferentes.

Esses nomes ajudam a identificar em qual etapa da comunicação os dados se encontram.

### Analogia

📦 Envio de uma encomenda

Imagine que você compra um produto pela internet.

Durante o processo ele pode receber nomes diferentes:

* Produto
* Encomenda
* Carga
* Entrega

Embora o conteúdo seja o mesmo, o nome muda conforme a etapa do transporte.

Na rede acontece exatamente a mesma coisa.

Os dados continuam sendo os mesmos, porém recebem nomes diferentes conforme atravessam as camadas.

### Frase para decorar

✅ PDU = nome dos dados em cada camada da comunicação.

---

# PDU no Modelo OSI

| Camada       | PDU                               |
| ------------ | --------------------------------- |
| Aplicação    | Dados (Data)                      |
| Apresentação | Dados (Data)                      |
| Sessão       | Dados (Data)                      |
| Transporte   | Segmento (TCP) ou Datagrama (UDP) |
| Rede         | Pacote (Packet)                   |
| Enlace       | Quadro (Frame)                    |
| Física       | Bits                              |

---

# Fluxo das PDUs

Durante o encapsulamento:

```text
Dados
↓
Segmento
↓
Pacote
↓
Quadro (Frame)
↓
Bits
```

Durante o desencapsulamento ocorre o processo inverso:

```text
Bits
↑
Quadro (Frame)
↑
Pacote
↑
Segmento
↑
Dados
```

---

# Entendendo Cada PDU

## Dados (Data)

### O que é?

Informação criada pela aplicação.

### Exemplos

* Mensagem do WhatsApp
* E-mail
* Foto
* Vídeo
* Página Web

### Analogia

📝 Carta escrita antes de ser colocada no envelope.

---

## Segmento (Segment)

### O que é?

PDU da Camada de Transporte.

Responsável por dividir grandes quantidades de dados em partes menores.

### Analogia

📦 Mudança residencial

Em vez de transportar tudo em uma única caixa gigante, os objetos são divididos em várias caixas menores.

---

## Pacote (Packet)

### O que é?

PDU da Camada de Rede.

Recebe informações de endereçamento IP.

### Analogia

🗺️ GPS

O pacote recebe o endereço de origem e destino para encontrar o caminho correto.

---

## Quadro (Frame)

### O que é?

PDU da Camada de Enlace.

Recebe os endereços MAC de origem e destino.

### Analogia

🏢 Entrega dentro de um condomínio

Além do endereço da rua, é necessário identificar corretamente o bloco e o apartamento.

---

## Bits

### O que é?

PDU da Camada Física.

Representa os sinais transmitidos pela rede.

### Analogia

💡 Interruptor

Possui apenas dois estados:

* Ligado = 1
* Desligado = 0

Toda comunicação digital é convertida em sequências de 0 e 1.

---

# Importância da PDU

A identificação das PDUs permite compreender:

* Como os dados trafegam pela rede.
* Em qual camada os dados estão.
* Como ocorre o encapsulamento.
* Como ocorre o desencapsulamento.
* Como localizar problemas durante a comunicação.

### Frase para decorar

✅ Dados → Segmento → Pacote → Quadro → Bits

✅ Essa é a sequência mais importante para provas e certificações.

# Encapsulamento e Desencapsulamento

## O que é Encapsulamento?

Encapsulamento é o processo de adicionar informações de controle aos dados antes que eles sejam enviados pela rede.

Cada camada adiciona seu próprio cabeçalho contendo informações necessárias para que os dados cheguem corretamente ao destino.

Essas informações podem incluir:

* Endereço IP
* Endereço MAC
* Número de porta
* Controle de erros
* Controle de sessão

### Analogia

📦 Envio pelos Correios

Imagine que você deseja enviar um produto para outra cidade.

Durante o envio são adicionadas várias informações:

* Caixa
* Etiqueta
* Endereço do destinatário
* Código de rastreamento

Quanto mais o pacote avança no processo, mais informações são adicionadas para garantir a entrega correta.

Na rede acontece exatamente a mesma coisa.

### Frase para decorar

✅ Encapsulamento = adicionar informações aos dados.

---

# Como Funciona o Encapsulamento

Os dados descem pelas camadas da rede.

Cada camada adiciona seu próprio cabeçalho.

### Camada de Aplicação

Cria os dados.

### Exemplo

💬 Mensagem enviada no WhatsApp:

"Olá, tudo bem?"

Nesse momento a informação é apenas um dado.

---

### Camada de Transporte

Adiciona informações do protocolo TCP ou UDP.

### Informações adicionadas

* Porta de origem
* Porta de destino
* Controle da comunicação

### Resultado

Dados → Segmento

### Analogia

📦 Dividir uma mudança em várias caixas menores para facilitar o transporte.

---

### Camada de Rede

Adiciona o endereço IP de origem e destino.

### Informações adicionadas

* IPv4 ou IPv6
* Roteamento

### Resultado

Segmento → Pacote

### Analogia

🗺️ Colocar o endereço da cidade e da rua na encomenda.

---

### Camada de Enlace

Adiciona o endereço MAC de origem e destino.

### Informações adicionadas

* MAC de origem
* MAC de destino

### Resultado

Pacote → Quadro (Frame)

### Analogia

🏢 Informar bloco e apartamento dentro de um condomínio.

---

### Camada Física

Converte os dados em sinais elétricos, ópticos ou sem fio.

### Resultado

Frame → Bits

### Analogia

🚚 O caminhão finalmente sai para realizar a entrega.

---

# Fluxo do Encapsulamento

```text
Dados
↓
Segmento
↓
Pacote
↓
Quadro (Frame)
↓
Bits
```

---

# O que é Desencapsulamento?

Desencapsulamento é o processo inverso.

Quando os dados chegam ao destino, cada camada remove as informações adicionadas durante o encapsulamento.

O objetivo é entregar apenas os dados originais para a aplicação.

### Analogia

📦 Recebendo uma encomenda

Quando a encomenda chega:

1. Você remove a embalagem externa.
2. Remove a etiqueta.
3. Remove a proteção interna.
4. Acessa o produto.

Na rede acontece a mesma coisa.

Cada camada remove suas informações até restarem apenas os dados originais.

### Frase para decorar

✅ Desencapsulamento = remover informações dos dados.

---

# Fluxo do Desencapsulamento

```text
Bits
↑
Quadro (Frame)
↑
Pacote
↑
Segmento
↑
Dados
```

---

# Exemplo Completo

Imagine que você envia uma mensagem pelo WhatsApp:

💬 "Bom dia"

### Origem

Aplicação cria os dados.

↓

Transporte adiciona TCP ou UDP.

↓

Rede adiciona IP.

↓

Enlace adiciona MAC.

↓

Física transmite os bits.

---

### Destino

Bits são recebidos.

↓

MAC é analisado e removido.

↓

IP é analisado e removido.

↓

TCP ou UDP é analisado e removido.

↓

A mensagem chega ao WhatsApp.

↓

Usuário lê:

💬 "Bom dia"

---

# Resumo para Memorizar

✅ Encapsulamento adiciona cabeçalhos.

✅ Desencapsulamento remove cabeçalhos.

✅ TCP/UDP adicionam informações de transporte.

✅ IP adiciona endereço lógico.

✅ MAC adiciona endereço físico.

✅ Dados → Segmento → Pacote → Frame → Bits.

✅ Bits → Frame → Pacote → Segmento → Dados.

# Segmentação de Dados

## O que é?

Segmentação é o processo de dividir grandes volumes de dados em partes menores para facilitar a transmissão pela rede.

Em vez de enviar um arquivo inteiro de uma única vez, a rede divide esse arquivo em vários segmentos menores.

Esses segmentos são enviados separadamente e posteriormente reorganizados no destino.

### Analogia

🚚 Mudança residencial

Imagine que você precisa transportar todos os móveis de uma casa.

Seria muito difícil colocar tudo dentro de uma única caixa gigante.

O mais eficiente é dividir os objetos em várias caixas menores.

Na rede acontece a mesma coisa.

Um arquivo grande é dividido em várias partes menores para facilitar o transporte.

### Frase para decorar

✅ Segmentação = dividir dados grandes em partes menores.

---

# Por que a Segmentação é Necessária?

Sem segmentação:

❌ Maior risco de perda de dados.

❌ Retransmissão de arquivos inteiros em caso de falha.

❌ Menor eficiência da rede.

Com segmentação:

✅ Melhor aproveitamento da rede.

✅ Maior velocidade de transmissão.

✅ Mais facilidade para corrigir erros.

✅ Retransmissão apenas da parte perdida.

### Analogia

📚 Entregar um livro inteiro ou vários capítulos separados.

Se um capítulo for perdido, basta reenviar aquele capítulo.

Não é necessário reenviar o livro inteiro.

---

# Como Funciona a Segmentação?

Imagine um vídeo de 500 MB.

Antes da transmissão ele é dividido em centenas ou milhares de pequenos segmentos.

Cada segmento recebe:

* Numeração
* Controle de sequência
* Informações de origem
* Informações de destino

No destino os segmentos são reorganizados na ordem correta.

### Exemplo

📦 Segmento 1

📦 Segmento 2

📦 Segmento 3

📦 Segmento 4

...

Todos são enviados separadamente.

Ao chegar ao destino são montados novamente.

### Analogia

🧩 Quebra-cabeça

Cada peça é enviada separadamente.

No final todas as peças são reunidas para formar a imagem completa.

---

# Segmentação no TCP

## O que acontece?

O protocolo TCP realiza a segmentação dos dados e controla a entrega.

### Funções

* Dividir os dados
* Numerar os segmentos
* Confirmar recebimento
* Reenviar segmentos perdidos

### Analogia

📦 Correios com rastreamento

Cada caixa possui um código.

Se uma caixa for extraviada:

🔄 Apenas aquela caixa é reenviada.

---

# Segmentação no UDP

## O que acontece?

O UDP também envia os dados em partes menores.

Porém não realiza controle rigoroso de entrega.

### Características

* Mais rápido
* Menor controle
* Sem confirmação de recebimento

### Analogia

📻 Rádio ao vivo

A transmissão continua mesmo que uma pequena parte seja perdida.

---

# Benefícios da Segmentação

### Eficiência

Permite melhor utilização da rede.

### Controle de Erros

Facilita identificar partes perdidas.

### Retransmissão

Permite reenviar apenas os segmentos que apresentaram falha.

### Organização

Mantém os dados estruturados durante a comunicação.

---

# Exemplo Prático

Imagine que você envia um vídeo pelo WhatsApp.

O vídeo não é enviado como um único bloco.

Ele é dividido em centenas ou milhares de segmentos.

Cada segmento percorre a rede.

Ao chegar ao destino:

* Os segmentos são reorganizados.
* O vídeo é reconstruído.
* O destinatário consegue assistir normalmente.

### Analogia

🎬 Filme em várias partes

Você recebe:

* Parte 1
* Parte 2
* Parte 3
* Parte 4

Quando todas chegam, o filme fica completo.

---

# Relação entre Segmentação e Encapsulamento

Primeiro ocorre a segmentação.

Depois ocorre o encapsulamento.

### Fluxo

```text
Dados
↓
Segmentação
↓
Segmentos
↓
Encapsulamento
↓
Pacotes
↓
Frames
↓
Bits
```

### Frase para decorar

✅ Primeiro divide.

✅ Depois encapsula.

---

# Resumo para Memorizar

✅ Segmentação divide dados grandes em partes menores.

✅ Ocorre na Camada de Transporte.

✅ TCP controla e confirma os segmentos.

✅ UDP envia sem confirmação.

✅ Facilita correção de erros.

✅ Permite retransmitir apenas a parte perdida.

✅ Segmentação acontece antes do encapsulamento.

# Multiplexação (MUX) e Demultiplexação (DEMUX)

## O que é Multiplexação (MUX)?

Multiplexação é a técnica que permite que vários tipos de dados compartilhem o mesmo meio de transmissão simultaneamente.

Em uma rede, diferentes aplicações podem utilizar o mesmo cabo, a mesma fibra óptica ou a mesma conexão Wi-Fi ao mesmo tempo.

### Analogia

🛣️ Rodovia

Imagine uma rodovia onde circulam:

* 🚗 Carros
* 🚌 Ônibus
* 🚚 Caminhões
* 🚑 Ambulâncias

Todos utilizam a mesma estrada, mas possuem destinos diferentes.

Na rede acontece a mesma coisa.

Diferentes aplicações utilizam a mesma infraestrutura de rede ao mesmo tempo.

### Frase para decorar

✅ Multiplexação = vários dados compartilhando o mesmo caminho.

---

# Por que a Multiplexação é Necessária?

Sem multiplexação:

❌ Cada aplicação precisaria de um cabo exclusivo.

❌ Alto custo de infraestrutura.

❌ Baixo aproveitamento da rede.

Com multiplexação:

✅ Melhor aproveitamento dos recursos.

✅ Redução de custos.

✅ Compartilhamento eficiente da infraestrutura.

---

# Exemplo Prático

Imagine que no seu computador você está:

* 🌐 Navegando na internet
* 🎵 Ouvindo música online
* 💬 Conversando no WhatsApp Web
* 📧 Recebendo e-mails

Todas essas aplicações utilizam a mesma conexão de rede.

A multiplexação permite que todos esses dados trafeguem simultaneamente.

### Analogia

🏢 Prédio comercial

Várias empresas utilizam o mesmo elevador.

Cada pessoa possui um destino diferente, mas todas compartilham o mesmo recurso.

---

# Como a Multiplexação Funciona?

A Camada de Transporte utiliza números de portas para identificar cada aplicação.

### Exemplos

| Serviço | Porta |
| ------- | ----- |
| HTTP    | 80    |
| HTTPS   | 443   |
| DNS     | 53    |
| SMTP    | 25    |

Essas portas ajudam a identificar qual aplicação enviou ou receberá os dados.

### Analogia

🏠 Condomínio

O endereço do prédio é o mesmo.

O número do apartamento identifica para quem a encomenda deve ser entregue.

Na rede:

* IP = endereço do prédio
* Porta = número do apartamento

### Frase para decorar

✅ Porta = identifica a aplicação.

---

# O que é Demultiplexação (DEMUX)?

Demultiplexação é o processo inverso.

Quando os dados chegam ao destino, a rede identifica para qual aplicação cada informação deve ser entregue.

### Analogia

📬 Carteiro

O carteiro chega ao prédio com várias correspondências.

Cada carta possui um apartamento diferente.

Ele separa cada correspondência e entrega ao destinatário correto.

A demultiplexação faz exatamente isso.

### Frase para decorar

✅ Demultiplexação = separar e entregar os dados para a aplicação correta.

---

# Exemplo Prático

Imagine que seu computador recebe ao mesmo tempo:

📧 Um e-mail

🌐 Dados de um site

💬 Mensagens do WhatsApp

🎵 Dados de uma música online

Todos chegam pela mesma interface de rede.

A demultiplexação analisa as portas e entrega cada informação para o programa correto.

### Resultado

* Navegador recebe os dados do site.
* WhatsApp recebe as mensagens.
* Cliente de e-mail recebe os e-mails.
* Aplicativo de música recebe o áudio.

---

# Multiplexação e Demultiplexação no TCP/IP

## Origem

As aplicações geram os dados.

↓

A multiplexação identifica cada aplicação utilizando portas.

↓

Os dados são enviados pela rede.

## Destino

Os dados chegam pela interface de rede.

↓

A demultiplexação analisa as portas.

↓

Os dados são entregues para a aplicação correta.

### Fluxo

```text id="h5t2qf"
Aplicações
↓
Multiplexação (MUX)
↓
Rede
↓
Demultiplexação (DEMUX)
↓
Aplicações
```

---

# Exemplo do Dia a Dia

Imagine um aeroporto.

### Multiplexação

✈️ Passageiros de vários destinos utilizam o mesmo aeroporto.

### Demultiplexação

🛄 Ao chegar ao destino, cada passageiro segue para sua esteira de bagagem, portão ou conexão correta.

O aeroporto é compartilhado, mas cada pessoa chega ao lugar certo.

---

# Relação com a Segmentação

A sequência lógica da comunicação é:

```text id="v2e4xp"
Dados
↓
Segmentação
↓
Multiplexação
↓
Transmissão
↓
Demultiplexação
↓
Reorganização dos Dados
```

### Analogia

📦 Transportadora

1. A carga é dividida em várias caixas (Segmentação).
2. As caixas de vários clientes compartilham o mesmo caminhão (Multiplexação).
3. O caminhão realiza a entrega.
4. As caixas são separadas por destinatário (Demultiplexação).
5. O cliente monta novamente seus produtos (Reorganização).

---

# Resumo para Memorizar

✅ Multiplexação = juntar vários fluxos de dados no mesmo meio de transmissão.

✅ Demultiplexação = separar os dados no destino.

✅ Utilizam números de portas para identificar aplicações.

✅ Permitem que várias aplicações compartilhem a mesma conexão.

✅ Multiplexação junta.

✅ Demultiplexação separa.


# 🌐 Padrão Ethernet IEEE 802.3 nas Redes Locais

## O que é?

O IEEE 802.3 é o padrão que define como ocorre a comunicação em redes Ethernet cabeadas.

Ele estabelece regras para:

* Transmissão de dados.
* Formato dos quadros (frames).
* Utilização de endereços MAC.
* Velocidade da comunicação.
* Funcionamento das redes locais (LAN).

### Exemplo

Quando um computador envia dados para outro através de um switch utilizando cabo de rede, normalmente está utilizando o padrão Ethernet IEEE 802.3.

---

## O que é o IEEE?

### O que significa?

**IEEE** (Institute of Electrical and Electronics Engineers) é uma organização internacional responsável pela criação de diversos padrões tecnológicos.

### Exemplos de padrões conhecidos

* IEEE 802.3 → Ethernet
* IEEE 802.11 → Wi-Fi
* IEEE 802.15 → Bluetooth

### Frase para decorar

✅ IEEE cria os padrões.
✅ Ethernet é definido pelo padrão 802.3.

---

## Características da Ethernet

### Utiliza Endereços MAC

Cada dispositivo possui um endereço físico único chamado MAC Address.

### Utiliza Quadros (Frames)

Na Camada de Enlace os dados são transportados em quadros.

### Alta Compatibilidade

Permite equipamentos de fabricantes diferentes trabalharem juntos.

### Escalabilidade

Pode ser utilizada em pequenas ou grandes redes.

### Baixo Custo

Tornou-se o padrão mais utilizado em redes locais.

---

## Estrutura Simplificada de um Frame Ethernet

Um quadro Ethernet normalmente contém:

* Endereço MAC de Origem.
* Endereço MAC de Destino.
* Tipo de Protocolo.
* Dados.
* Verificação de Erros (FCS).

### Exemplo

📦 Encomenda dos Correios:

* Remetente = MAC de Origem
* Destinatário = MAC de Destino
* Conteúdo = Dados
* Código de Rastreio = Controle de Integridade

---

## Evolução das Velocidades Ethernet

### Ethernet

* 10 Mbps

### Fast Ethernet

* 100 Mbps

### Gigabit Ethernet

* 1000 Mbps (1 Gbps)

### 10 Gigabit Ethernet

* 10 Gbps

### Velocidades atuais

Existem padrões Ethernet de:

* 25 Gbps
* 40 Gbps
* 100 Gbps
* 400 Gbps

Principalmente em datacenters e provedores.

---

## CSMA/CD

### O que é?

CSMA/CD significa:

**Carrier Sense Multiple Access with Collision Detection**

Era o mecanismo utilizado nas antigas redes Ethernet compartilhadas para detectar colisões.

### Como funcionava?

1. O dispositivo escutava o meio.
2. Se estivesse livre, transmitia.
3. Se ocorresse colisão, aguardava um tempo aleatório.
4. Tentava transmitir novamente.

### Exemplo

Imagine duas pessoas tentando falar ao mesmo tempo em uma sala.

As duas param, aguardam alguns segundos e tentam novamente.

### Observação

Nas redes modernas com switches Full Duplex praticamente não existem colisões, tornando o CSMA/CD pouco utilizado atualmente.

### Frase para decorar

✅ CSMA/CD foi criado para controlar colisões na Ethernet antiga.

---

## Ethernet e o Modelo OSI

### Camada Física

Responsável por:

* Cabos.
* Conectores.
* Sinais elétricos ou ópticos.

### Camada de Enlace

Responsável por:

* Endereços MAC.
* Quadros Ethernet.
* Controle de acesso ao meio.

### Frase para decorar

✅ Ethernet atua principalmente nas Camadas 1 e 2 do Modelo OSI.

---

## Analogia para Memorizar

Imagine uma cidade com ruas e regras de trânsito.

🚗 Os veículos representam os dados.

🛣️ As ruas representam os cabos.

🏠 Os endereços representam os MAC Addresses.

🚦 As regras de trânsito representam o padrão Ethernet.

Sem as regras, cada motorista dirigiria de uma forma diferente.

Com o padrão Ethernet, todos seguem as mesmas regras de comunicação.

---

## 🧠 Resumo para Memorizar

✅ IEEE 802.3 define o padrão Ethernet.

✅ Ethernet é o padrão mais utilizado em redes locais.

✅ Utiliza MAC Address para identificar dispositivos.

✅ Utiliza Frames na Camada de Enlace.

✅ Atua principalmente nas Camadas 1 e 2 do Modelo OSI.

✅ CSMA/CD controlava colisões nas redes antigas.

✅ Equipamentos de fabricantes diferentes conseguem se comunicar graças ao padrão Ethernet.


