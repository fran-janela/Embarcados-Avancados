#  👁 Entrega 1

O objetivo dessa entrega é automatizarmos a compilação e deploy de novos programas para o `target`. Para isso, teremos que criar um Makefile que deve ser capaz de compilar e fazer o deploy de programa. Para isso temos diversas opções, sendo alguma delas:

- Transferência de arquivo via ssh: [scp](http://www.hypexr.org/linux_scp_help.php)
- Montar do pasta do `target` no `host` remota via ssh: [sshfs](https://en.wikipedia.org/wiki/SSHFS)
- Via [gdb server](https://www.linux.com/news/remote-cross-target-debugging-gdb-and-gdbserver)
    - executa no `target` um gdb server que possibilita ao `host` transferir e debugar um binário.

Note que todas as soluções demandam de conexão com de rede, para isso,
siga o roteiro: [Info HPS Ethernet](Embarcados-Avancados/info-HPS-ethernet/).

## Rubrica:

!!! info
    Você deve fazer as entregas pelo repositório do github criado no classroom:
    
    - https://classroom.github.com/a/fGUME066
    
    Crie uma pasta chamada: `1-makefile` e faça a entrega por ela

> Para testar, modifique o makefile do `BlinkLed`

- A (novo) 
    - Faz o uboot bootar via tftp: https://ece453.engr.wisc.edu/u-boot-script/
- B
    - Debuga um programar no target (via gdbserver)
- C
    - Criou um Makefile que compila o código e faz o deploy para o `target` de um programa
    - Via Makefile consegue executar o binário no `target`
        - *make run* / *make deploy*
    - Coloca um `README.md` na pasta que explica como usa e o que faz.
- D 
    - Entregou somente os tutoriais
- I
    - Não entregou nada
