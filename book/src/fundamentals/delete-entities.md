# Delete Entities

Deleting an entity means take it away from the entities' storage as well as deleting all its components.

```rust, noplaypen
world.borrow::<AllStorages>.delete(entity_id);
```

`delete` takes a single `EntityId` of the entity you want to delete. It returns a `bool`, `true` if the entity was present in the entities' storage before calling the method.