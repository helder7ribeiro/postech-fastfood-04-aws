# FastFood - Infraestrutura AWS

Este projeto contém a infraestrutura Terraform para o sistema FastFood na AWS.

## Estrutura do Projeto

```
├── RDS/                    # Módulo para recursos de banco de dados
│   ├── main.tf            # Recursos RDS principais
│   ├── variables.tf       # Variáveis do módulo
│   ├── provider.tf        # Configuração do provider AWS
│   ├── backend.tf         # Configuração do backend S3
│   └── README.md          # Documentação do módulo
├── .github/               # Configurações do GitHub
└── README.md              # Este arquivo
```

## Módulos Disponíveis

### RDS
- **Localização**: `RDS/`
- **Descrição**: Provisiona instância PostgreSQL RDS
- **Documentação**: [RDS/README.md](RDS/README.md)

## Próximos Módulos Planejados

- **EC2**: Instâncias para aplicação
- **VPC**: Rede e subnets
- **Security Groups**: Regras de segurança
- **Load Balancer**: Balanceador de carga
- **S3**: Armazenamento de objetos

## Como Usar

1. Navegue para o módulo desejado:
   ```bash
   cd RDS
   ```

2. Inicialize o Terraform:
   ```bash
   terraform init
   ```

3. Planeje as mudanças:
   ```bash
   terraform plan
   ```

4. Aplique a infraestrutura:
   ```bash
   terraform apply
   ```

## Pré-requisitos

- Terraform instalado
- AWS CLI configurado
- Bucket S3 para backend (configurado em cada módulo)
