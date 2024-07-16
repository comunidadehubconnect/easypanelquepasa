<p align="center">
<img src="https://cwmkt.com.br/wp-content/uploads/2024/04/logo_github.png" width="240" />
<p align="center">Seja bem-vindo ao Guia de Instalação EasyPanel Evolution 2.0 🚀</p>
</p>
  
<p align="center"> 
<a href="https://hubconnect.top" target="_blank">👉 Participe da Comunidade HubConnect 👈</a>
</p>

<hr />
<hr />

## Comando para Instalar EasyPanel

```bash
curl -sSL https://get.easypanel.io | sh
```

Adicione nome de Project

![48098522-0c485df00f5cadb0d329061c35fee46c](https://github.com/cwmkt/easypanelevotypebot/assets/91642837/b72c1359-91ca-4bf6-9fb1-32525ba5747b)

Clique na aba Templates

![48098535-90f9b4f370bb8b06cfd7e4acf0ee0f97](https://github.com/cwmkt/easypanelevotypebot/assets/91642837/03c1830c-621c-40b3-94ee-93eb568c8d2e)

Va ate final da pagina

![image](https://github.com/comunidadehubconnect/easypanelwoofedcrm/assets/91642837/828a9e88-45f2-4b6b-98f1-ab4f164d2889)

Adicione codigo abaixo dentro do Schema

![image](https://github.com/comunidadehubconnect/easypanelwoofedcrm/assets/91642837/74b97f33-e5d2-495d-aaba-25bb8b433adf)

```bash
{
    "services": [
        {
            "type": "app",
            "data": {
                "projectName": "quepasa",
                "serviceName": "quepasa",
                "source": {
                    "type": "image",
                    "image": "codeleaks/quepasa"
                },
                "domains": [
                    {
                        "host": "$(EASYPANEL_DOMAIN)",
                        "port": 31000
                    }
                ],
                "env": "DOMAIN=https://$(PRIMARY_DOMAIN) \nEMAIL=seu@email.com \nTZ=America/Sao_Paulo \nAPP_ENV=production \nNODE_ENV=production \nWEBHOOK_QUEPASA=https://$(PRIMARY_DOMAIN)/webhook/quepasa \nWEBHOOK_TESTE_QUEPASA=https://$(PRIMARY_DOMAIN)/webhook-test/quepasa \nAPP_TITLE=Servidor NoCodeLeaks \nQUEPASA_CONTAINER_NAME=NoCodeLeaks \nQUEPASA_HOST_NAME=quepasa \nQUEPASA_MEMORY_LIMIT=4096M \nQUEPASA_EXTERNAL_PORT=31000 \nQUEPASA_INTERNAL_PORT=31000 \nWEBAPIPORT=31000 \nWEBSOCKETSSL=true \nSIGNING_SECRET=BLA!2#BlA123bLA1 \nQUEPASA_BASIC_AUTH_USER=seu@email.com \nQUEPASA_BASIC_AUTH_PASSWORD=TESTE \nMETRICS_HOST= \nMETRICS_PORT=9392 \nMIGRATIONS=/builder/migrations \nDEBUGJSONMESSAGES=false \nHTTPLOGS=false",
                "mounts": [
                    {
                        "type": "volume",
                        "name": "quepasa_lab_volume",
                        "mountPath": "/opt/quepasa"
                    },
                    {
                        "type": "volume",
                        "name": "quepasa_lab_builder_volume",
                        "mountPath": "/builder"
                    }
                ]
            }
        }
    ]
}

```

### Baixe os arquivos no Git oficial 

```bash
https://github.com/nocodeleaks/quepasa
```

![image](https://github.com/cwmkt/dockerquepasa/assets/91642837/9a69690d-8c7e-4ed9-a5ca-ce9632a05456)


Suba pasta \quepasa-main\src do Quepasa dentro volume

```bash
/etc/easypanel/projects/nomedoprojeto/quepasa/volumes/quepasa_lab_volume
```

![image](https://github.com/user-attachments/assets/54469215-e3d3-444a-9db4-a55e53f5e732)


Acesse: seudominio.com.br/setup

Faça seu cadastro

Pronto tudo Funcionando ✅😎

Creditos: Andre Marques
