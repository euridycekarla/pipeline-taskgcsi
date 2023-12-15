<h1 align="center"> pipeline-taskgcsi </h1>
<div style="display: flex; justify-content: center;">
    <img src="https://github.com/euridycekarla/pipeline-taskgcsi/assets/91157048/d870f424-eb67-4ff7-8802-c4aa1d2c67f6"  width="100px"/>
</div>

<h2> Atividade de GCSI<br></br>

Criação da Pipeline com Jenkins</h2>

Uhuuuul, última atividade de gerência e configuração  de serviços de internet

<h3>Permissões de acesso</h3>

 Para iniciar a configuração é necessário ter acesso no diretório para evitar problemas futuros na configuração do jenkins.


 * Para entrar no diretório acesse o seguinte comando no terminal:   `cd var/run`

* Permita o acesso do arquivo **docker.sock**: `sudo chmod 777 docker.sock`

* Verifique as permissões do arquivo: `ls-la | grep docker.sock`


<h2>Vamos criar a pipeline com Jenkins:</h2>

* É necessário que você um projeto com Jenkinsfile na sua máquina, e construa a aplicação com o **docker compose up**.
<br></br>


 <img src="https://github.com/euridycekarla/pipeline-taskgcsi/assets/91157048/c4da8c0d-bbd1-4940-bbf7-27d31cc84cb5"/>

<br></br>

* Quando a aplicação for construída você receberá uma senha criptograda no terminal que servirá de acesso no Jenkins.

  Que servirá de acesso como senha neste seguinte painel:
  <img src="https://github.com/euridycekarla/pipeline-taskgcsi/assets/91157048/31e5d394-942e-4fcd-9a25-d5a95fb713ea"/>
O nome do usário é de sua escolha. A senha é gerada e aparece no terminal.

* Em seguida, crie uma tarefa, no canto superior esquerdo, será exibido uma tela como essa abaixo, no painel de controle  crie uma nova pipeline:

  <img src="https://github.com/euridycekarla/pipeline-taskgcsi/assets/91157048/6ca0cbc1-1072-4c16-8ef4-4343b6840313"/>

* Adicione uma descrição na sua pipeline:
  <img src="https://github.com/euridycekarla/pipeline-taskgcsi/assets/91157048/ca650041-8c80-4820-b89f-75aab38122d2"/>

* Congifure os dados do seu reposítório:
<img src="https://github.com/euridycekarla/pipeline-taskgcsi/assets/91157048/10d4e89d-a14d-4189-8c62-a4898f733a30"/>

* Depois de configurar, vá em `construir agora` no canto superior direito:
<img src="https://github.com/euridycekarla/pipeline-taskgcsi/assets/91157048/9b3fa609-0ce1-43e9-907d-e9f572556743"/>

 * Clique em `Open Blue Ocean` para ver o andamento do build e o test do seu projeto de pipeline.
  <img src="https://github.com/euridycekarla/pipeline-taskgcsi/assets/91157048/2da1e131-1c6e-4ab4-af33-01d82a74c69d"/>

  * Clique no processo que você deu run e veja as etapas:

    <img src="https://github.com/euridycekarla/pipeline-taskgcsi/assets/91157048/b01fa360-e766-47d0-93c4-ca14df1bbf5d"/>

Se tudo der certo, você verá uma tela como estas. Tudo verdinho e no terminal no final, terá um `OK`. Seu código rodou certinho com o jenkins na pipeline.
