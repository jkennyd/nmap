# Tabela de Parâmetros do Nmap

| Parâmetro                      | Utilidade                                                                 |
|-------------------------------|---------------------------------------------------------------------------|
| `-sS`                          | Varredura TCP SYN (rápida e furtiva)                                      |
| `-sT`                          | Varredura TCP completa (connect scan)                                     |
| `-sU`                          | Varredura de portas UDP                                                   |
| `-sN`                          | Varredura TCP Null (sem flags)                                            |
| `-sF`                          | Varredura TCP FIN                                                         |
| `-sX`                          | Varredura TCP Xmas                                                        |
| `-sA`                          | Verifica se uma porta está filtrada com ACK                               |
| `-sW`                          | Descobre firewalls usando TCP Window                                      |
| `-sM`                          | Varredura TCP Maimon                                                      |
| `-sL`                          | Apenas lista os hosts (sem varredura)                                     |
| `-sn`                          | Ping scan (detecta hosts ativos, sem varrer portas)                       |
| `-Pn`                          | Ignora detecção de host (assume que todos estão ativos)                   |
| `-p <portas>`                  | Define portas específicas para escanear (ex: `-p 22,80,443`)              |
| `-p-`                          | Escaneia todas as 65535 portas                                            |
| `-F`                           | Fast scan: escaneia somente portas mais comuns                            |
| `--top-ports <N>`             | Escaneia as N portas mais comuns                                          |
| `-T<0-5>`                      | Ajusta velocidade/agressividade (0 = mais lento, 5 = mais rápido)         |
| `-A`                           | Habilita detecção de SO, versão, scripts e traceroute                     |
| `-O`                           | Detecta sistema operacional                                               |
| `--osscan-guess`              | Força palpite de SO mesmo que não seja preciso                            |
| `-sV`                          | Detecta versão de serviços nas portas abertas                             |
| `--version-all`               | Tenta todos os métodos de detecção de versão                              |
| `--version-light`            | Detecção de versão mais leve e rápida                                     |
| `--version-intensity <0-9>`  | Ajusta agressividade na detecção de versão                                |
| `-v`                           | Modo verboso                                                              |
| `-vv`, `-vvv`                  | Verbosidade ainda maior                                                   |
| `-d`                           | Modo debug (mais detalhes de execução)                                    |
| `-oN <arquivo>`               | Salva saída no formato normal                                             |
| `-oX <arquivo>`               | Salva saída no formato XML                                                |
| `-oG <arquivo>`               | Salva saída no formato grepable                                           |
| `-oA <prefixo>`               | Salva em todos os formatos (normal, XML e grepable)                       |
| `-iL <arquivo>`               | Usa uma lista de IPs/hosts de um arquivo                                  |
| `-iR <N>`                     | Escaneia N hosts aleatórios                                               |
| `--exclude <hosts>`          | Exclui IPs/hosts do scan                                                  |
| `--excludefile <arquivo>`    | Exclui IPs listados em um arquivo                                         |
| `--script <nome ou categoria>`| Executa scripts NSE (ex: `--script http-enum`)                            |
| `--script-args <args>`       | Argumentos personalizados para scripts NSE                                |
| `--script-help <script>`     | Mostra ajuda sobre um script específico                                   |
| `--traceroute`               | Executa traceroute até o host                                             |
| `--reason`                   | Mostra o motivo da detecção de estado de portas                           |
| `--open`                     | Mostra somente portas abertas                                             |
| `--max-retries <N>`          | Define máximo de tentativas para cada host                                |
| `--host-timeout <tempo>`     | Tempo máximo para escanear um host (ex: `--host-timeout 5m`)              |
| `--min-rate <pps>`           | Define taxa mínima de pacotes por segundo                                 |
| `--max-rate <pps>`           | Define taxa máxima de pacotes por segundo                                 |
| `--spoof-mac <mac|prefixo>`  | Faz spoofing de endereço MAC                                              |
| `-6`                           | Escaneia via IPv6                                                         |
| `-R`                           | Resolve nomes DNS reversos                                                |
| `-n`                           | Não resolve nomes DNS                                                     |
| `--dns-servers <ip1,ip2>`     | Usa servidores DNS específicos                                            |

