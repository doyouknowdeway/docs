### Таблица пользователя

```
user:
	<id>,
	<role_id>,
	<reg_date>
```

### Таблица профиля пользователя
```
profile:
	<id>,
	<login>,
	<email>,
	<pass_hash>,
	<firstname>,
	<secondname>,
	<lastname>
```

### Таблица ролей пользователя
```
roles:
	<id>,
	<name>
```

### Таблица инвентаря
```
items:
	<id>,
	<name>,
	<description>,
	<per_hour_cost>,
	<season_type>,
	<age_type>,
	<count>
```

```
season_type:
	<id>,
	<name>
```

```
age_type:
	<id>,
	<name>
```

### Таблица общего заказа
```
order:
	<id>,
	<profile_id>,
	<status_id>
	<order_time>,
	<dest_time>,
	<exp_time>,
	<total_price>
```
>	<total_price> = (exp_time - dest_time) * rent_item.item_id.per_hour_cost

```
order_status:
	<id>,
	<name>
```

### Таблица аренды товара
```
rent_item:
	<item_id>,
	<order_id>
```

