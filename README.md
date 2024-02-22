# MoneyMinder


## Requisitos

- [ ] CRUD de movimentações (Gastos ou receitas)
- [ ] CRUD Categorias
- [ ] Dashbosrd (Mostra a onde você esta gastando mais e etc.)
- [ ] Altenticação de Usuarios

## Endpoints

### Categorias


`GET` /categoria

Lista todas as catecorias do sistema.

---
`GET` /categoria/{id}

Retorna os detalhes de uma categoria com o `id` informado.

**códico de status**

`200` sucesso
`404` id não encontrado 

---
`POST` /categoria

Cadatrar uma nova categoria.

| campo | tipo | obrigatório | descrição
| ----- | ---- | :-----------: | ---------
|nome|string|✅|Um nome curto para indendificar a categoria
|icone|string|❌|O nome do icone conforma biblioteca do material desing

**códico de status**

`201` criado com sucesso
`400` validação falhou 

---
`DELETE`/categoria/{id}

**códico de status**

`204` Apagado com sucesso
`404` id não encontrado 

---
`PUT`/categoria/{id}

**códico de status**

`200` sucesso
`404` id não encontrado
`400` validação falhou  

**Scheme**
```js

{
    "id": 1,
    "nome": "Alimentação",
    "icone": "fast-food"

}

```


