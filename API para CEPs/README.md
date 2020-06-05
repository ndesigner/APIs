# API CEP via VIACEP

### Utiliza��o:

**Include**

> Include no arquivo CepInfo.class.php

#### _Base:_

> $cep = new CEP(NUMERO-CEP);

#### _Para buscar apenas uma informa��o_

> $cep->getOneInfo(informa��o)

V�lidos: ['cep', 'logradouro', 'bairro', 'localidade', 'uf', 'ibge']

#### _Para buscar mais de uma informa��o_

> $cep->getMoreInfos([array])

V�lidos: ['cep', 'logradouro', 'bairro', 'localidade', 'uf', 'ibge']

#### _Para buscar todas as informa��es que a API retorna_

> $cep->getData();

# Importante

- Para CEPs inv�lidos retornar�:
> **CEP inv�lido.**

- Para CEPs inexistentes retornar�: 
> **CEP inexistente.**