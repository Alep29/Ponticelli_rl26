Prerequisiti

    Ambiente Linux Ubuntu configurato sul computer host.

    Docker installato e funzionante.

    Cartella di progetto locale contenente la sottocartella docker_scripts con i relativi file di configurazione eseguibili.

Come avviare il container

    Aprire il terminale e spostarsi nella directory del progetto: cd ~/Ponticelli_rl26

    Lanciare lo script di avvio: ./docker_scripts/docker_run_container.sh

    Selezionare l'immagine ros2_lab_image (digitando 1) e, alla richiesta della cartella, inserire Ponticelli_rl26 per montare il volume condiviso.

Verifica del completamento del Task 2

    Dal terminale del container attivo (user@...), creare il file di test digitando: touch /home/user/ros2_ws/src/test_persistence.txt

    Chiudere l'ambiente Docker digitando: exit

    Dal terminale locale, confermare che il file sia stato salvato sul computer fisico digitando: ls -a src/
