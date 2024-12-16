# Phishing Attack Simulation

## Objetivo
Simular um ataque phishing buscando obter a senha de contas do instagram.com utiliando o setoolkit do Kali Linux.

## Requisitos
- Kali Linux

## Passos e comandos
- Abra o terminal no Kali Linux
- ```sudo su```
- Digite a senha sudo (admin) do linux
- ![sudo su](/imgs/sudo%20su.png)
- ```setoolkit```
- ![setoolkit](/imgs/setoolkit.png)
- Opção "Website Attack Vectors": ```2```
- ![Website Attack](/imgs/Website%20Attack.png)
- Opção "Credencial Harvester Attack Method": ```3```
- ![Credential Harvester Attack Method](/imgs/Credential%20Harvester%20Attack%20Method.png)
- Opção "Site Clone": ```2```
- ![Site Cloner](/imgs/Site%20Cloner.png)
- Será usado a própria máquina linux como host do site clonado, ou seja, o IP entre "[]": ```Enter```
- ![host IP](/imgs/host%20IP.png)
- Será clonado o instagram.com: ```https://www.instagram.com```
- ![url to clone](/imgs/url%20to%20clone.png)
- Em um navegador web entre no IP do host config, exemplo: ```192.168.3.38```
- ![site clonado no navegador](/imgs/site%20clonado%20no%20navegador.png)
- Insira um e-mail (username) e senha (password) de testes nos respectivos campos do site
- No terminal do Kali linux será exibido o fluxo de informações enviadas pelo navegador e entre elas será apontado possíveis 
e-mail (username) e sennha (password) informadas ao site clonado
- ![console result](/imgs/console%20result.png)

## Observações
- O exemplo apresentou alguns erros entre os retornos do setoolkit. Suponho que seja questão de compatibilidade versões do navegador.
- Foi possível identificar de forma clara apenas o username, pois a password foi apresentada de forma criptografada pelo navegador, 
como forma de segurança. Porém foi notado, depois de alguns teste, que os caracteres apresentados após o último ":" são a senha informada, 
no caso do teste "123456"