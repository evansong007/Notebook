### subject
- trapdoor`furniture`
- key`artefacts`
- tree`furniture`
- axe`artefacts`
- potion`artefacts`
- elf`characters`
- coin`artefacts`
- log`artefacts`
- river`furniture`
- ground`furniture`
- shovel`artefacts`
- horn`artefacts`

### consumed
- key`artefacts`:romve form current location,add to storeroom
- tree`furniture`:romve form current location,add to storeroom
- potion`artefacts`:romve form current location,add to storeroom
- health`player`:player health -1
- coin`artefacts`:romve form current location,add to storeroom
- log`artefacts`:romve form current location,add to storeroom
- ground`furniture`:romve form current location,add to storeroom
- `null`
- `location`: remove path form current location to target location

### produced
- cellar`location`:add path form current location to target location
- log`artefacts`:remove other location, add to current location
- health`player`:player health +1
- `null`:
- shovel`artefacts`:remove other location, add to current location
- clearing`location`:add path form current location to target location
- hole`furniture`:remove other location, add to current location
- gold`artefacts`:remove other location, add to current location
- lumberjack`characters`:remove other location, add to current location

### consumed
- consumed(`artefacts`):romve form current location,add to storeroom
- consumed(`furniture`):romve form current location,add to storeroom
- consumed(`location`):remove path form currentlocation to target location
- consumed(`player`):player health -1
- consumed(`characters`):romve form current location,add to storeroom
- consumed(`null`):do nothing

### produced
- procduced(`location`):add path form current location to target location
- produced(`artefacts`):remove other location, add to current location
- produced(`player`):health + 1
- produced(`furniture`):remove other location, add to current location
- produced(`characters`):remove other location, add to current location
- produced(`null`):do nothing