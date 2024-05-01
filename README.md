# Docker-Aula-30-04

Para executar o container de leitura, abra o cmd do wsl e rode o seguinte comando:

```docker run -v /home/scalabr/rxTx/pastaCompartilhada:/pastaCompartilhada:ro -it ubuntu sh```

em seguida, entre na pasta referente a pasta criada utilizando ```cd pastaCompartilhada```

e rode o comando ```touch teste.txt```

caso o erro ```touch: cannot touch 'teste.txt': Read-only file system``` significa que a função de somente leitura está configurada corretamente.

Para criar o container de leitura e escrita, execute o seguinte comando:

```docker run -v /home/scalabr/rxTx/pastaCompartilhada:/pastaCompartilhada -it ubuntu sh```

Ao entrar na pasta criada utilizando ```cd pastaCompartilhada``` será possível executar comandos de criação e leitura livremente.
