# Atividades-Beecrowd
Atividades propostas pelo Professor Carlos dentro do site judge.beecrowd.com

## Nível 1
### Atividade 2603
<img width="1080" height="307" alt="Image" src="https://github.com/user-attachments/assets/cc4f5975-1350-4b50-939b-f585b6c75904" />


Código usado para resolução:

``` sql
SELECT
    name,
    street
FROM 
    customers
WHERE
    city = 'Porto Alegre'
```

### Atividade 2607
<img width="1081" height="307" alt="Image" src="https://github.com/user-attachments/assets/bd1bf395-6c4c-461e-8285-0b71cff9719e" />

Código usado para resolução:

```sql
SELECT
    city
FROM providers
ORDER BY city
```


## Nível 2
### Atividade 2604
<img width="670" height="306" alt="Image" src="https://github.com/user-attachments/assets/d544698b-4a3f-4e45-b458-ee32f9aa795d" />
Código usado para resolução:

```sql
SELECT 
    id,
    name
FROM
    products
WHERE
    price < 10 or price >100
```

### 2619
<img width="1079" height="308" alt="Image" src="https://github.com/user-attachments/assets/7e2f1724-db2f-465e-bb02-b8d173423222" />
Código usado para resolução:

```sql
    products.name,
    providers.name,
    products.price
FROM products
JOIN 
    providers ON products.id_providers = providers.id
JOIN
    categories on products.id_categories = categories.id
WHERE
    products.price > 1000
    AND categories.name = 'Super Luxury'
```

## Nível 3
### Atividade  2610
<img width="1081" height="307" alt="Image" src="https://github.com/user-attachments/assets/cf2dad23-6780-460e-8974-2e1764bec558" />


Código usado para resolução:

```sql
SELECT
    ROUND(SUM(price)/COUNT(price), 2) as media_total
FROM products;
```

###  Atividade 2618
<img width="1079" height="304" alt="Image" src="https://github.com/user-attachments/assets/b6b60c80-7b35-43c6-befb-23ed20cd6a7d" />


Código usado para resolução:

```sql
SELECT
    products.name,
    providers.name,
    categories.name
FROM products
JOIN
    providers ON products.id_providers = providers.id
JOIN
    categories ON products.id_categories = categories.id
WHERE
    providers.name = 'Sansul SA'
    AND categories.name = 'Imported';
```

## Nível 4
### Atividade 2602
<img width="677" height="311" alt="Image" src="https://github.com/user-attachments/assets/9a369ea3-cfdc-4d13-a529-9770a2c3c1b6" />

Código usado para resolução:

```sql
select name
from 
    customers
where 
    state = 'RS'
```
