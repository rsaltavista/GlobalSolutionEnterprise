# GlobalSolutionEnterprise


Entrega da materia de enterprise.
### Link do vídeo no youtube: https://youtu.be/jJWR5z9EMys
# DoarHero
## Descrição do projeto
    Nosso projeto é um aplicativo que tem como objetivo facilitar a 
    doação de alimentos para pessoas em situação de vulnerabilidade. 
    Através da plataforma, os usuários podem se cadastrar como 
    doadores e buscar por instituições ou indivíduos que estejam 
    precisando de alimentos.
    A plataforma permite que os doadores visualizem uma lista de 
    pedidos de alimentos feitos por pessoas necessitadas. Eles podem 
    selecionar um pedido e fazer a doação correspondente, seja de 
    alimentos não perecíveis, alimentos frescos ou até mesmo refeições 
    prontas. A entrega dos alimentos pode ser combinada diretamente 
    entre o doador e o beneficiário, ou pode ser feita por meio de uma 
    instituição parceira que atue na distribuição de alimentos.
    Nosso objetivo é promover a solidariedade e ajudar a combater a 
    fome, facilitando o processo de doação de alimentos de forma direta 
    e simples. Através dessa plataforma, esperamos conectar doadores 
    generosos com pessoas que necessitam de auxílio alimentar, 
    proporcionando uma maneira eficiente e efetiva de ajudar a 
    comunidade.

## Instruções para rodar a url da nossa API rest!
    Para testar a nossa aplicação nós colocamos o localhost em público, porém é temporário, para isso usamos o localtunnel, os passos a seguir mostram como usar:

    1) Abra o CMD(Prompt de comando);


    2) Instalação:

    "npm install -g localtunnel"


    3) Quando o localtunnel estiver instalado globalmente, basta usar o ltcomando para iniciar o túnel:

    "lt --port 8080"


    4) Ele se conectará ao servidor do túnel, configurará o túnel e informará qual url usar para o teste.

    5) no final da url, colocar /usuarios ou /ongs ou /doacoes. exemplo: https://api.example.com/usuarios ou https://api.example.com/ongs ou https://api.example.com/doacoes 

    Observação: teve vezes que ao fechar o cmd o localhost parava de funcionar. então por precaução não fechar o cmd.

    É isso! 

# Lista de Endpoints
## ***Usuário***
## GET 
https://api.example.com/usuarios
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará. 
### Descrição: Consulta a lista de usuários cadastrados.
### Exemplo de solicitação: N/A
### Exemplo de resposta:
    [
        {
            "id": "1",
            "nome": "Cristina",
            "email": "cristina@gmail.com",
            "senha": "familia1212",
            "rua": "rua reliquia",
            "cidade": "são paulo",
            "numero": "223",
            "cep": "02514333",
            "complemento": "perto da igreja"
        },
    ...
    ]

## POST
https://api.example.com/usuarios
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará. 
### Descrição: Cadastra um novo usuário.
### Exemplo de solicitação:
    
        {
            "nome": "fabricio",
            "email": "fabricio@gmail.com",
            "senha": "futset222",
            "rua": "rua esmeralda",
            "cidade": "São paulo",
            "numero": "44",
            "cep": "020323",
            "complemento": "perto da padaria"
        }
    
### Exemplo de resposta:
       
        {
            "nome": "fabricio",
            "email": "fabricio@gmail.com",
            "senha": "futset222",
            "rua": "rua esmeralda",
            "cidade": "São paulo",
            "numero": "44",
            "cep": "020323",
            "complemento": "perto da padaria"
        }
    
## PUT 
https://api.example.com/usuarios/2
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará. 
### Descrição: Atualiza informações sobre o usuário cadastrado.
### Exemplo de solicitação:
    
        {
            "nome": "fabricio",
            "email": "fabricio@gmail.com",
            "senha": "futset222",
            "rua": "rua araguari 9987",
            "cidade": "São paulo",
            "numero": "44",
            "cep": "020323",
            "complemento": "perto da padaria"
        }
### Exemplo de resposta:
        {
            "nome": "fabricio",
            "email": "fabricio@gmail.com",
            "senha": "futset222",
            "rua": "rua araguari 9987",
            "cidade": "São paulo",
            "numero": "44",
            "cep": "020323",
            "complemento": "perto da padaria"
        }
## DELETE 
https://api.example.com/usuarios/2
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará. 
### Descrição: Deleta o usuário selecionado. No caso deletará o usuário com o id = 2.
### Exemplo de solicitação: N/A
### Exemplo de resposta: N/A  
## ***Ong***
## GET
https://api.example.com/ongs
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará.
## Descrição: Consulta a lista de ONGs cadastradas.
## Exemplo de solicitação: N/A
## Exemplo de resposta:
    [
        {
            "id": 22,
            "nome": "mundo sem fome",
            "descricao": "Temos o objetivo de diminuir a fome no mundo",
            "rua": "rua caplin 223",
            "cidade": "São Paulo",
            "numero": "264",
            "cep": "0003234"
        },
    ...
    ]
## Post
https://api.example.com/ongs
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará.
## Descrição: Cadastra uma nova ONG.
## Exemplo de solicitação:
    {
        "nome": "Floresta da Paz",
        "descricao": "Esta ong tem foco ajudar e fornecer alimentos para creches que no tem condies de auto-sustento",
        "rua": "Rua maria das dores",
        "cidade": "Sao Paulo",
        "numero": "905",
        "cep": "02433503"
    }
## Exemplo de resposta:
    {
        "nome": "Floresta da Paz",
        "descricao": "Esta ong tem foco ajudar e fornecer alimentos para creches que no tem condies de auto-sustento",
        "rua": "Rua maria das dores",
        "cidade": "Sao Paulo",
        "numero": "905",
        "cep": "02433503"
    }

## PUT
https://api.example.com/ongs/2
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará.
### Descrição: Atualiza informações sobre a ONG cadastrada.
### Exemplo de solicitação:
    {
        "nome": "Floresta da Paz",
        "descricao": "Esta ong tem foco ajudar e fornecer alimentos para creches que no tem condies de auto-sustento",
        "rua": "Rua Silva",
        "cidade": "Sao Paulo",
        "numero": "905",
        "cep": "02433503"
    }
### Exemplo de resposta:
    {
        "nome": "Floresta da Paz",
        "descricao": "Esta ong tem foco ajudar e fornecer alimentos para creches que no tem condies de auto-sustento",
        "rua": "Rua Silva",
        "cidade": "Sao Paulo",
        "numero": "905",
        "cep": "02433503"
    }
## DELETE 
https://api.example.com/ongs/2
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará. 
### Descrição: Deleta o usuário selecionado. No caso deletará a Ong com o id = 2.
### Exemplo de solicitação: N/A
### Exemplo de resposta: N/A

## ***Doação***
## GET
https://api.example.com/doacoes
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará.
## Descrição: Consulta a lista de doações cadastradas.
## Exemplo de solicitação: N/A
## Exemplo de resposta:
    [
        {
            "id": 1,
            "descricao": "Doacao de Carnes",
            "dataDoacao": "2021-03-14",
            "rua": "Rua Jose Fernando",
            "cidade": "Sao Paulo",
            "numero": "12",
            "cep": "02452002",
            "usuario": null,
            "ong": null
        }
    ...
    ]
## Post
https://api.example.com/docaoes
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará.
### OBS: Para informar uma data, é necessário utilizar a formatação: yyyy-mm-dd(Ano-Mês-Dia).
## Descrição: Cadastra uma nova Doação.
## Exemplo de solicitação:
    {
        "descricao": "Doação de fruta",
        "dataDoacao": "2023-02-12",
        "rua": "Rua reliquia",
        "cidade": "São Paulo",
        "numero": "44",
        "cep": "02514221",
        "usuario": null,
        "ong": null
    }
## Exemplo de resposta:
    
    {
        "id": 2,
        "descricao": "Doação de fruta",
        "dataDoacao": "2023-02-12",
        "rua": "Rua reliquia",
        "cidade": "São Paulo",
        "numero": "44",
        "cep": "02514221",
        "usuario": null,
        "ong": null
    }
    

## PUT
https://api.example.com/doacoes/2
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará.
### OBS: Para informar uma data, é necessário utilizar a formatação: yyyy-mm-dd(Ano-Mês-Dia).
### Descrição: Atualiza informações sobre a Doacao cadastrada.
### Exemplo de solicitação:
    {
        "descricao": "Doação de pipocas",
        "dataDoacao": "2023-02-12",
        "rua": "Rua reliquia",
        "cidade": "São Paulo",
        "numero": "44",
        "cep": "02514221",
        "usuario": null,
        "ong": null
    }
### Exemplo de resposta:
    {
        "descricao": "Doação de pipocas",
        "dataDoacao": "2023-02-12",
        "rua": "Rua reliquia",
        "cidade": "São Paulo",
        "numero": "44",
        "cep": "02514221",
        "usuario": null,
        "ong": null
    }
## DELETE 
https://api.example.com/doacoes/2
### Observação: no lugar de 'api.example.com', substituir pela url que o localtunnel informará. 
### Descrição: Deleta o usuário selecionado. No caso deletará a Doação com o id = 2.
### Exemplo de solicitação: N/A
### Exemplo de resposta: N/A


## Diagrama de classe:
![Imagem do WhatsApp de 2023-06-06 à(s) 21 10 52](https://github.com/rsaltavista/GlobalSolutionEnterprise/assets/92685333/1f93a2d1-0914-4d6a-8ba5-37488662cd98)







