- Spawn one spawn of type `Spawn1` with the name `Upgrader1` and `[WORK, CARRY, MOVE]` abilities

```js
Game.spawns['Spawn1'].spawnCreep( [WORK, CARRY, MOVE], 'Upgrader1' );
```


- Add a role in memory for both `Harvester1` and `Upgrader1`
```js
Game.creeps['Harvester1'].memory.role = 'harvester';
Game.creeps['Upgrader1'].memory.role = 'upgrader';
```

- Add a role on spawn :
```js
Game.spawns['Spawn1'].spawnCreep( [WORK, CARRY, MOVE], 'Builder1',
    { memory: { role: 'builder' } } );
```