# Phishing Attack Simulation

## Objetivo
Simular um ataque phishing buscando obter a senha de contas do instagram.com utiliando o setoolkit do Kali Linux.

## Requisitos
- Kali Linux

## Passos e comandos
- Abra o terminal no Kali Linux
- ```sudo su```
- Digite a senha sudo (admin) do linux
- Snapshot 1
- ```setoolkit```
- Snapshot c
- Opção "Website Attack Vectors": ```2```
- Snapshot 2
- Opção "Credencial Harvester Attack Method": ```3```
- Snapshot 3
- Opção "Site Clone": ```2```
- Snapshot 4
- Será usado a própria máquina linux como host do site clonado, ou seja, o IP entre "[]": ```Enter```
- Será clonado o instagram.com: ```https://www.instagram.com```
- Print 2
- Em um navegador web entre no IP do host config, exemplo: ```192.168.3.38```
- Print do navegador
- Insira um e-mail (username) e senha (password) de testes nos respectivos campos do site
- No terminal do Kali linux será exibido o fluxo de informações enviadas pelo navegador e entre elas será apontado possíveis e-mail (username) e sennha (password) informadas ao site clonado
- Snapshot 5

## Observações
- O exemplo apresentou alguns erros entre os retornos do setoolkit. Suponho que seja questão de compatibilidade versões do navegador.
- Foi possível identificar de forma clara apenas o username, pois a password foi apresentada de forma criptografada pelo navegador, como forma de segurança.
