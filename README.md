📌 Sobre o projeto 10/11/2026

O objetivo deste laboratório foi praticar comandos de diagnóstico de rede e entender como aplicá-los em cenários de suporte a clientes e administração de infraestrutura.

A atividade também reforçou a relação entre os comandos de troubleshooting e as camadas do modelo OSI, com foco nas camadas de rede, transporte e aplicação.

🎯 Objetivos

Praticar comandos utilizados na solução de problemas de rede.

Investigar conectividade, rotas, portas e comunicação com serviços.

Relacionar os testes técnicos a situações comuns de suporte e operações de TI.

Utilizar acesso remoto SSH em uma instância EC2 Linux.

☁️ Ambiente utilizado

Plataforma: Amazon Web Services (AWS)

Serviço: Amazon EC2

Sistema operacional: Amazon Linux

Acesso remoto: SSH

Terminal: Linux

📸 Evidências do laboratório

1. Instância Amazon EC2

<img width="1681" height="818" alt="image" src="https://github.com/user-attachments/assets/4332b3bc-01e7-469b-88f6-50c04f0b4dfb" />


Instância EC2 utilizada no laboratório.

2. Conexão SSH com a instância Linux

<img width="1506" height="313" alt="image" src="https://github.com/user-attachments/assets/b302d044-8202-48b6-951a-df082b2e61b4" />


Acesso remoto à instância Amazon Linux por SSH.

3. Teste de conectividade com Ping
<img width="824" height="377" alt="image" src="https://github.com/user-attachments/assets/5f5b13ab-f025-439e-906a-903e40b93f90" />



Teste de conectividade IP utilizando ICMP.

4. Análise de rota com Traceroute

<img width="1448" height="209" alt="image" src="https://github.com/user-attachments/assets/a1ee2e16-3a55-4881-9328-2c08b3d4c01b" />


Análise do caminho percorrido pelos pacotes até o destino.

5. Verificação de conexões com Netstat

<img width="1161" height="211" alt="image" src="https://github.com/user-attachments/assets/a0a9c023-a794-4249-95ae-8d1b59067092" />


Consulta de conexões e portas no sistema.

6. Teste de porta com Telnet

<img width="1821" height="175" alt="image" src="https://github.com/user-attachments/assets/bff28287-ee04-4c80-a7c7-05829dd8b33a" />


Teste de estabelecimento de conexão TCP com uma porta específica.

7. Teste HTTP/HTTPS com Curl
<img width="1897" height="890" alt="image" src="https://github.com/user-attachments/assets/497c1aac-20a6-453b-bed2-4b465a07ac54" />
<img width="1739" height="918" alt="image" src="https://github.com/user-attachments/assets/03275ca3-bd01-4e6a-a206-a7c326520ad4" />
<img width="1882" height="978" alt="image" src="https://github.com/user-attachments/assets/6b7801e8-5460-41d1-b7d3-7d291aa0a0a8" />

Teste de comunicação com um serviço web.

💻 Comandos praticados

Comando

Finalidade

Exemplo

SSH

Acesso remoto a uma instância Linux

ssh -i labsuser.pem ec2-user@<ip-publico>

Ping

Verificar conectividade IP

ping 8.8.8.8 -c 5

Traceroute

Analisar o caminho dos pacotes

traceroute 8.8.8.8

Netstat

Consultar conexões e portas

netstat -tp

Telnet

Testar conexão TCP em uma porta

telnet www.google.com 80

Curl

Testar comunicação HTTP/HTTPS

curl -vLo /dev/null https://aws.com

Atenção: os exemplos são referências para estudo. O endereço IP, o destino e as opções devem ser ajustados conforme o ambiente. O Telnet foi utilizado para diagnóstico de conectividade, não como método seguro de administração remota.

🌐 Relação com o modelo OSI

Durante o laboratório, os comandos foram relacionados às seguintes camadas:

Camada 3 – Rede: Ping e Traceroute, para investigar conectividade IP e caminho dos pacotes.

Camada 4 – Transporte: Netstat e Telnet, para analisar conexões e testar portas TCP.

Camada 7 – Aplicação: Curl, para verificar a comunicação com serviços web.

📚 Aprendizados

A prática ajudou a reforçar uma abordagem organizada de troubleshooting: começar verificando a conectividade, analisar o caminho até o destino, conferir conexões e portas e, por fim, testar a resposta do serviço de aplicação.

Esses conhecimentos são úteis em atividades de suporte técnico, operações de redes, administração Linux e infraestrutura em nuvem.

📂 Estrutura do repositório

troubleshooting-redes-aws/
│
├── README.md
│
└── images/
    ├── 01-instancia-ec2.png
    ├── 02-conexao-ssh.png
    ├── 03-ping.png
    ├── 04-traceroute.png
    ├── 05-netstat.png
    ├── 06-telnet.png
    └── 07-curl.png

Tópicos: AWS · Amazon EC2 · Linux · Redes de Computadores · Troubleshooting · Modelo OSI · SSH · ICMP · TCP · HTTP · HTTPS
