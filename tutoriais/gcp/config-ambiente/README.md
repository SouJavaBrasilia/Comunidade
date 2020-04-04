# Iniciando com Google Cloud Plataform

## Crie seu cadastro

 [Link](https://console.cloud.google.com/)

## Configure o SDK

 [Link](https://cloud.google.com/sdk/docs/quickstarts)
 
## Testando

    $ git clone https://github.com/GoogleCloudPlatform/getting-started-java
    $ cd getting-started-java/helloworld-servlet
    
### Rodando local
   
    $ mvn jetty:run-exploded

Abra o browser no endereço http://localhost:8080
    
### Implantando no AppEgine

Liste seus projetos com:

    $ gcloud projects list

Execute
    
    $ gcloud config set project <YOUR_PROJECT_ID>
    $ mvn appengine:deploy    
    $ gcloud app browse
    
Abra o painel do app engine e confira o resultado
    
### Dicas

* Certifique o seu projeto estar ativo
* Certifique do serviço cloud build estar ativo e com permissão
* Desabilite o serviço após o teste para não faturar