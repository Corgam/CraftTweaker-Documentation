# Expansion for MCEntityType

Additional methods for easier modification of entity-related loot tables.

## Methods

### addDrop

Adds an [IItemStack](/vanilla/api/items/IItemStack) to the drops of this entity.

Return Type: void

```zenscript
MCEntityType.addDrop(uniqueId as string, stack as IItemStack) as void
```

| Параметр | Тип                                         | Description                        |
| -------- | ------------------------------------------- | ---------------------------------- |
| uniqueId | string                                      | A unique id for the loot modifier. |
| stack    | [IItemStack](/vanilla/api/items/IItemStack) | The stack to add to the drops.     |


### addDrops

Adds a list of [IItemStack](/vanilla/api/items/IItemStack)s to the drops of this entity.

Return Type: void

```zenscript
MCEntityType.addDrops(uniqueId as string, stacks as IItemStack[]) as void
```

| Параметр | Тип                                           | Description                        |
| -------- | --------------------------------------------- | ---------------------------------- |
| uniqueId | string                                        | A unique id for the loot modifier. |
| stacks   | [IItemStack](/vanilla/api/items/IItemStack)[] | The stacks to add to the drops.    |


### addLootModifier

Adds an [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) to the current entity.

Return Type: void

```zenscript
MCEntityType.addLootModifier(name as string, modifier as ILootModifier) as void
```

| Параметр | Тип                                                        | Description                             |
| -------- | ---------------------------------------------------------- | --------------------------------------- |
| name     | string                                                     | The name of the loot modifier.          |
| modifier | [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) | The loot modifier to add to the entity. |


### addPlayerOnlyDrop

Adds an [IItemStack](/vanilla/api/items/IItemStack) to the drops of this entity, but only if the entity was killed by a player.

Return Type: void

```zenscript
MCEntityType.addPlayerOnlyDrop(uniqueId as string, stack as IItemStack) as void
```

| Параметр | Тип                                         | Description                        |
| -------- | ------------------------------------------- | ---------------------------------- |
| uniqueId | string                                      | A unique id for the loot modifier. |
| stack    | [IItemStack](/vanilla/api/items/IItemStack) | The stack to add to the drops.     |


### addPlayerOnlyDrops

Adds a list of [IItemStack](/vanilla/api/items/IItemStack)s to the drops of this entity, but only if the entity was killed by a player.

Return Type: void

```zenscript
MCEntityType.addPlayerOnlyDrops(uniqueId as string, stacks as IItemStack[]) as void
```

| Параметр | Тип                                           | Description                        |
| -------- | --------------------------------------------- | ---------------------------------- |
| uniqueId | string                                        | A unique id for the loot modifier. |
| stacks   | [IItemStack](/vanilla/api/items/IItemStack)[] | The stacks to add to the drops.    |


### addPlayerOnlyLootModifier

Adds an [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) to the current entity that fires only if the entity was killed by a player.

Return Type: void

```zenscript
MCEntityType.addPlayerOnlyLootModifier(name as string, modifier as ILootModifier) as void
```

| Параметр | Тип                                                        | Description                             |
| -------- | ---------------------------------------------------------- | --------------------------------------- |
| name     | string                                                     | The name of the loot modifier.          |
| modifier | [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) | The loot modifier to add to the entity. |


### addWeaponAndPlayerOnlyDrop

Adds an [IItemStack](/vanilla/api/items/IItemStack) to the drops of this entity, but only if the entity was killed by a player with the given weapon.

 Additional parameters that further specify the weapon, such as NBT, count, or damage, are ignored.

Return Type: void

```zenscript
MCEntityType.addWeaponAndPlayerOnlyDrop(uniqueId as string, weapon as IItemStack, stack as IItemStack) as void
```

| Параметр | Тип                                         | Description                                          |
| -------- | ------------------------------------------- | ---------------------------------------------------- |
| uniqueId | string                                      | A unique id for the loot modifier.                   |
| weapon   | [IItemStack](/vanilla/api/items/IItemStack) | The weapon that needs to be used to kill the entity. |
| stack    | [IItemStack](/vanilla/api/items/IItemStack) | The stack to add to the drops.                       |


### addWeaponAndPlayerOnlyDrops

Adds a list of [IItemStack](/vanilla/api/items/IItemStack)s to the drops of this entity, but only if the entity was killed by a player with the given weapon.

 Additional parameters that further specify the weapon, such as NBT, count, or damage, are ignored.

Return Type: void

```zenscript
MCEntityType.addWeaponAndPlayerOnlyDrops(uniqueId as string, weapon as IItemStack, stacks as IItemStack[]) as void
```

| Параметр | Тип                                           | Description                                          |
| -------- | --------------------------------------------- | ---------------------------------------------------- |
| uniqueId | string                                        | A unique id for the loot modifier.                   |
| weapon   | [IItemStack](/vanilla/api/items/IItemStack)   | The weapon that needs to be used to kill the entity. |
| stacks   | [IItemStack](/vanilla/api/items/IItemStack)[] | The stacks to add to the drops.                      |


### addWeaponAndPlayerOnlyLootModifier

Adds an [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) to the current entity that fires only if the entity was killed by a player with the given weapon.

 Additional parameters that further specify the weapon, such as NBT, count, or damage, are ignored.

Return Type: void

```zenscript
MCEntityType.addWeaponAndPlayerOnlyLootModifier(name as string, weapon as IItemStack, modifier as ILootModifier) as void
```

| Параметр | Тип                                                        | Description                                          |
| -------- | ---------------------------------------------------------- | ---------------------------------------------------- |
| name     | string                                                     | The name of the loot modifier.                       |
| weapon   | [IItemStack](/vanilla/api/items/IItemStack)                | The weapon that needs to be used to kill the entity. |
| modifier | [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) | The loot modifier to add to the entity.              |


Adds an [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) to the current entity that fires only if the entity was killed by a player with the given weapon, optionally considering its damage.

 Additional parameters that further specify the weapon, such as NBT, or count, are ignored.

Return Type: void

```zenscript
MCEntityType.addWeaponAndPlayerOnlyLootModifier(name as string, weapon as IItemStack, matchDamage as boolean, modifier as ILootModifier) as void
```

| Параметр    | Тип                                                        | Description                                                    |
| ----------- | ---------------------------------------------------------- | -------------------------------------------------------------- |
| name        | string                                                     | The name of the loot modifier.                                 |
| weapon      | [IItemStack](/vanilla/api/items/IItemStack)                | The weapon that needs to be used to kill the entity.           |
| matchDamage | boolean                                                    | Whether to consider damage or not when identifying the weapon. |
| modifier    | [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) | The loot modifier to add to the entity.                        |


Adds an [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) to the current entity that fires only if the entity was killed by a player with the given weapon, optionally considering its damage and NBT data.

 Additional parameters that further specify the weapon, such as count, are ignored.

Return Type: void

```zenscript
MCEntityType.addWeaponAndPlayerOnlyLootModifier(name as string, weapon as IItemStack, matchDamage as boolean, matchNbt as boolean, modifier as ILootModifier) as void
```

| Параметр    | Тип                                                        | Description                                                      |
| ----------- | ---------------------------------------------------------- | ---------------------------------------------------------------- |
| name        | string                                                     | The name of the loot modifier.                                   |
| weapon      | [IItemStack](/vanilla/api/items/IItemStack)                | The weapon that needs to be used to kill the entity.             |
| matchDamage | boolean                                                    | Whether to consider damage or not when identifying the weapon.   |
| matchNbt    | boolean                                                    | Whether to consider NBT data or not when identifying the weapon. |
| modifier    | [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) | The loot modifier to add to the entity.                          |


### addWeaponOnlyDrop

Adds an [IItemStack](/vanilla/api/items/IItemStack) to the drops of this entity, but only if the entity was killed with the given weapon.

 Additional parameters that further specify the weapon, such as NBT, count, or damage, are ignored.

Return Type: void

```zenscript
MCEntityType.addWeaponOnlyDrop(uniqueId as string, weapon as IItemStack, stack as IItemStack) as void
```

| Параметр | Тип                                         | Description                                          |
| -------- | ------------------------------------------- | ---------------------------------------------------- |
| uniqueId | string                                      | A unique id for the loot modifier.                   |
| weapon   | [IItemStack](/vanilla/api/items/IItemStack) | The weapon that needs to be used to kill the entity. |
| stack    | [IItemStack](/vanilla/api/items/IItemStack) | The stack to add to the drops.                       |


### addWeaponOnlyDrops

Adds a list of [IItemStack](/vanilla/api/items/IItemStack)s to the drops of this entity, but only if the entity was killed with the given weapon.

 Additional parameters that further specify the weapon, such as NBT, count, or damage, are ignored.

Return Type: void

```zenscript
MCEntityType.addWeaponOnlyDrops(uniqueId as string, weapon as IItemStack, stacks as IItemStack[]) as void
```

| Параметр | Тип                                           | Description                                          |
| -------- | --------------------------------------------- | ---------------------------------------------------- |
| uniqueId | string                                        | A unique id for the loot modifier.                   |
| weapon   | [IItemStack](/vanilla/api/items/IItemStack)   | The weapon that needs to be used to kill the entity. |
| stacks   | [IItemStack](/vanilla/api/items/IItemStack)[] | The stacks to add to the drops.                      |


### addWeaponOnlyLootModifier

Adds an [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) to the current entity that fires only if the entity was killed with the given weapon.

 Additional parameters that further specify the weapon, such as NBT, count, or damage, are ignored.

Return Type: void

```zenscript
MCEntityType.addWeaponOnlyLootModifier(name as string, weapon as IItemStack, modifier as ILootModifier) as void
```

| Параметр | Тип                                                        | Description                                          |
| -------- | ---------------------------------------------------------- | ---------------------------------------------------- |
| name     | string                                                     | The name of the loot modifier.                       |
| weapon   | [IItemStack](/vanilla/api/items/IItemStack)                | The weapon that needs to be used to kill the entity. |
| modifier | [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) | The loot modifier to add to the entity.              |


Adds an [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) to the current entity that fires only if the entity was killed with the given weapon, optionally considering its damage.

 Additional parameters that further specify the weapon, such as NBT, or count, are ignored.

Return Type: void

```zenscript
MCEntityType.addWeaponOnlyLootModifier(name as string, weapon as IItemStack, matchDamage as boolean, modifier as ILootModifier) as void
```

| Параметр    | Тип                                                        | Description                                                    |
| ----------- | ---------------------------------------------------------- | -------------------------------------------------------------- |
| name        | string                                                     | The name of the loot modifier.                                 |
| weapon      | [IItemStack](/vanilla/api/items/IItemStack)                | The weapon that needs to be used to kill the entity.           |
| matchDamage | boolean                                                    | Whether to consider damage or not when identifying the weapon. |
| modifier    | [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) | The loot modifier to add to the entity.                        |


Adds an [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) to the current entity that fires only if the entity was killed with the given weapon, optionally considering its damage and NBT data.

 Additional parameters that further specify the weapon, such as count, are ignored.

Return Type: void

```zenscript
MCEntityType.addWeaponOnlyLootModifier(name as string, weapon as IItemStack, matchDamage as boolean, matchNbt as boolean, modifier as ILootModifier) as void
```

| Параметр    | Тип                                                        | Description                                                      |
| ----------- | ---------------------------------------------------------- | ---------------------------------------------------------------- |
| name        | string                                                     | The name of the loot modifier.                                   |
| weapon      | [IItemStack](/vanilla/api/items/IItemStack)                | The weapon that needs to be used to kill the entity.             |
| matchDamage | boolean                                                    | Whether to consider damage or not when identifying the weapon.   |
| matchNbt    | boolean                                                    | Whether to consider NBT data or not when identifying the weapon. |
| modifier    | [ILootModifier](/vanilla/api/loot/modifiers/ILootModifier) | The loot modifier to add to the entity.                          |


