---

# 📦 Explicação do Código de Controle de Estoque

Este código simples tem como objetivo **verificar se um produto está disponível no estoque**. A seguir, explicamos cada parte do código passo a passo:

---

## 📝 Código

```python
# Lista de produtos disponíveis no estoque
estoque = ["Camiseta", "Calça", "Tênis", "Boné", "Jaqueta"]

# Entrada do usuário
produto = input().strip()

# TODO: Verifique se o produto está no estoque:
if produto in estoque:
    print("Produto disponível")
else:
    print("Produto esgotado")
```

---

## 🔍 Explicação

### 1. Lista de Produtos

```python
estoque = ["Camiseta", "Calça", "Tênis", "Boné", "Jaqueta"]
```

* Aqui, criamos uma **lista chamada `estoque`** que contém os produtos atualmente disponíveis.

---

### 2. Entrada do Usuário

```python
produto = input().strip()
```

* O programa **espera o usuário digitar o nome de um produto**.
* `.strip()` remove **espaços em branco extras** no começo e fim da entrada, garantindo uma comparação mais precisa.

---

### 3. Verificação de Estoque

```python
if produto in estoque:
    print("Produto disponível")
else:
    print("Produto esgotado")
```

* O programa verifica se o produto digitado está **presente na lista `estoque`**.
* Se estiver, exibe: `"Produto disponível"`.
* Caso contrário, exibe: `"Produto esgotado"`.

---

## ✅ Exemplo de Uso

Entrada:

```
Camiseta
```

Saída:

```
Produto disponível
```

---

## 🚀 Sugestões de Melhorias

* Tornar a verificação **insensível a maiúsculas/minúsculas**:

  ```python
  if produto.lower() in [item.lower() for item in estoque]:
  ```

* Permitir que o usuário **adicione ou remova produtos do estoque**.

* Exibir todos os produtos disponíveis antes da entrada.

---
