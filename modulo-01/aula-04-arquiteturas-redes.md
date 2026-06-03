# Aula 04 - Arquiteturas de Redes, Convergência, QoS e Segurança

## 🎯 Objetivo da Aula

Compreender os modelos de comunicação utilizados nas redes modernas, os conceitos de escalabilidade, tolerância a falhas, qualidade de serviço (QoS), convergência, segurança e integração entre fabricantes.

---

# ☎️ Comunicação Baseada em Circuito

## O que é?

Modelo de comunicação que estabelece um caminho exclusivo entre origem e destino durante toda a transmissão.

## Características

- Canal dedicado.
- Comunicação contínua.
- Recursos reservados durante toda a conexão.
- Se o caminho falhar, a comunicação é interrompida.

## Exemplo

Imagine uma ponte reservada exclusivamente para dois carros.

Enquanto os carros utilizam a ponte, ninguém mais pode passar por ela.

Se a ponte cair:

❌ A comunicação é interrompida imediatamente.

## Exemplo Real

📞 Telefonia fixa tradicional.

## Resumo

✅ Caminho exclusivo.

❌ Baixa tolerância a falhas.

---

# 📦 Comunicação Baseada em Pacotes

## O que é?

Modelo utilizado nas redes modernas, onde os dados são divididos em pequenos pacotes antes da transmissão.

## Características

- Não existe caminho exclusivo.
- Os pacotes podem utilizar rotas diferentes.
- Maior flexibilidade.
- Melhor aproveitamento da infraestrutura.
- Maior tolerância a falhas.

## Exemplo

Você compra um guarda-roupa pela internet.

Ele é enviado em várias caixas:

📦 Caixa 1

📦 Caixa 2

📦 Caixa 3

Cada caixa pode seguir por um caminhão diferente.

Ao chegar ao destino, todas as partes são reunidas e montadas.

Na rede acontece o mesmo processo com os pacotes de dados.

## Exemplo Real

🌐 Internet

🌐 Redes TCP/IP

## Resumo

✅ Melhor utilização da rede.

✅ Maior tolerância a falhas.

---

# 🔄 Tolerância a Falhas (Fault Tolerance)

## O que é?

Capacidade da rede continuar funcionando mesmo quando ocorre alguma falha.

## Características

- Possui redundância.
- Possui caminhos alternativos.
- Aumenta a disponibilidade da rede.

## Exemplo

Uma empresa possui dois links de internet:

🌐 Link Vivo

🌐 Link Claro

Se um deles falhar:

✅ O outro continua funcionando.

## Frase para Decorar

> Quem tem 1 não tem nenhum. Quem tem 2 tem 1.

## Resumo

✅ Redundância.

✅ Continuidade dos serviços.

---

# 📈 Escalabilidade

## O que é?

Capacidade da infraestrutura crescer sem exigir uma reconstrução completa da rede.

## Características

- Planejamento para expansão.
- Facilidade de crescimento.
- Suporte para novos dispositivos e usuários.

## Exemplo

Uma empresa possui:

👨‍💻 10 funcionários atualmente.

Mas pretende crescer para:

👨‍💻 30 funcionários nos próximos meses.

A rede deve ser planejada para suportar essa expansão.

## Frase para Decorar

> Escalabilidade é pensar no crescimento antes que ele aconteça.

## Resumo

✅ Rede preparada para o futuro.

---

# 🚦 QoS (Quality of Service)

## O que é?

Mecanismo utilizado para priorizar determinados tipos de tráfego na rede.

## Para que serve?

Garantir que aplicações críticas tenham prioridade quando houver congestionamento.

## Características

- Reduz atrasos.
- Evita congestionamentos.
- Prioriza aplicações importantes.

## Exemplo

Em uma rodovia congestionada:

🚑 Ambulância

🚗 Carro comum

Quem recebe prioridade?

A ambulância.

Na rede acontece o mesmo processo.

## Exemplo de Prioridades

1. VoIP (telefonia)
2. Sistemas críticos
3. Navegação web
4. CFTV

## Frase para Decorar

> QoS = fila preferencial dos pacotes.

## Resumo

✅ Prioriza tráfego importante.

✅ Melhora desempenho das aplicações críticas.

---

# 🔒 Segurança em Redes

A segurança pode ser dividida em duas categorias principais:

- Segurança Física
- Segurança Lógica

---

## 🏢 Segurança Física

### O que é?

Proteção dos equipamentos e da infraestrutura.

### Exemplos

- Rack trancado.
- Sala de servidores.
- Controle de acesso físico.
- Câmeras de monitoramento.

### Objetivo

Evitar danos, furtos ou acessos indevidos aos equipamentos.

---

## 💻 Segurança Lógica

### O que é?

Proteção dos dados e sistemas da organização.

### Exemplos

- Senhas.
- Firewall.
- Antivírus.
- Controle de permissões.
- Políticas de acesso.

### Objetivo

Proteger informações e recursos digitais.

---

# 📜 PSI (Política de Segurança da Informação)

## O que é?

Conjunto de regras que define como os recursos tecnológicos devem ser utilizados dentro da organização.

## Exemplos

Define:

- Quem pode acessar sistemas.
- Quem pode alterar configurações.
- Quem pode visualizar determinadas informações.

## Objetivo

Padronizar e controlar o uso dos recursos de TI.

---

# ⚖️ LGPD

## O que é?

Lei Geral de Proteção de Dados.

Legislação brasileira criada para proteger os dados pessoais dos cidadãos.

## Exemplos de Dados Protegidos

- CPF
- Telefone
- E-mail
- Endereço
- Dados financeiros

## Objetivo

Garantir privacidade e proteção das informações pessoais.

## Resumo

✅ Empresas devem proteger os dados dos usuários.

---

# 🔄 Arquitetura sem Convergência

## O que é?

Cada serviço utiliza uma infraestrutura própria e independente.

## Exemplo

📞 Telefonia → Rede própria

📺 TV → Rede própria

💻 Computadores → Rede própria

Tudo separado.

## Características

- Maior custo.
- Maior complexidade.
- Menor aproveitamento dos recursos.

---

# 🌐 Arquitetura com Convergência

## O que é?

Vários serviços utilizam a mesma infraestrutura de rede.

## Exemplo

📞 VoIP

📹 CFTV

💻 Internet

📂 Compartilhamento de arquivos

Todos funcionando na mesma rede Ethernet/TCP-IP.

## Exemplo Lúdico

⚽ Imagine um campo de futebol.

Vários times utilizam o mesmo campo em horários diferentes.

O campo representa a infraestrutura da rede.

## Frase para Decorar

> Convergência = vários serviços utilizando a mesma rede.

## Benefícios

✅ Menor custo.

✅ Maior integração.

✅ Melhor aproveitamento da infraestrutura.

---

# 🏭 Multivendor

## O que é?

Utilização de equipamentos de fabricantes diferentes trabalhando na mesma rede.

## Exemplos

🔀 Switch Cisco

🔥 Firewall Fortinet

📶 Access Point Ubiquiti

Todos funcionando juntos.

## Exemplo Lúdico

Imagine pessoas de diferentes regiões do Brasil:

👨 Paulista

👨 Carioca

👨 Nordestino

Cada um possui seu sotaque.

Mesmo assim, todos falam português.

Na rede acontece algo semelhante.

Cada fabricante possui sua forma de configuração, mas todos utilizam padrões como:

- Ethernet
- TCP/IP
- IPv4
- IPv6

## Frase para Decorar

> Multivendor = fabricantes diferentes falando a mesma língua.

## Benefícios

✅ Maior flexibilidade.

✅ Melhor custo-benefício.

✅ Liberdade na escolha dos equipamentos.

---

# 🧠 Resumo para Memorizar

- Comunicação por circuito utiliza caminho exclusivo.
- Comunicação por pacotes divide os dados em partes menores.
- Tolerância a falhas utiliza redundância.
- Escalabilidade permite crescimento da rede.
- QoS prioriza tráfego importante.
- Segurança física protege equipamentos.
- Segurança lógica protege dados e sistemas.
- PSI define regras de utilização dos recursos.
- LGPD protege dados pessoais.
- Convergência permite vários serviços na mesma rede.
- Multivendor permite integrar equipamentos de fabricantes diferentes.
