# Phishing Attack Simulation

## Objetivo
Simular um ataque phishing buscando obter a senha de contas do instagram.com utiliando o setoolkit do Kali Linux.

## Requisitos
- Kali Linux

## Passos e comandos
- ```sudo su```
- Digite a senha sudo (admin) do linux
- Snapshot 1
- Opção "Website Attack Vectors": ```2```
- Snapshot 2
- Opção "Credencial Harvester Attack Method": ```3```
- Snapshot 3
- Opção "Site Clone": ```2```
- Snapshot 4
- Usaremos a própria máquina linux como host do site clonado, ou seja, o IP entre "[]": ```Enter```
- Clonaremos o instagram.com: ```https://www.instagram.com```
- Em um navegador web entramos no IP do host config, exemplo: ```192.168.3.38```
- Print do navegador
- No terminar do Kali linux será exibido o fluxo de informações enviadas pelo navegador e entre elas será apontado possíveis usernames e passwords
- Snapshot 5

## Observações
- O exemplo a cima apresentado apresentou alguns erros no console. Suponho que seja questão de compatibilidade com o navegador.
- Foi possível identificar de forma clara apenas o username, pois a password foi apresentada de forma criptografada pelo navegador, como forma de segurança.
