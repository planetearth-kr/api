# PlanetEarth API
오픈월드 타우니 지구서버 플래닛어스 공식 API 입니다. 모든 정보는 JSON 형식으로 반환됩니다.

### API Endpoint
Default parameters:
```
key=API_KEY : API에 접근하기 위한 인증 키입니다. 플래닛어스 공식 디스코드에서 문의를 통해 얻을 수 있습니다.
```

Example:
```
https://planetearth.kr/api/discord?key=JUSTANEXAMPLEKEY&name=Irochi_
```

### https://planetearth.kr/api/discord

Available parameters:
```
discord=DISCORD_ID : 디스코드 ID를 입력하면 디스코드 ID, UUID, 닉네임을 반환합니다.
uuid=UUID : UUID를 입력하면 디스코드 ID, UUID, 닉네임을 반환합니다.
name=IGN : 닉네임을 입력하면 디스코드 ID, UUID, 닉네임을 반환합니다.
```

Returns:
```
discord, uuid, name
```

### https://planetearth.kr/api/resident

Available parameters:
```
uuid=UUID : UUID를 입력하면 해당 유저의 정보를 반환합니다.
name=IGN : 닉네임을 입력하면 해당 유저의 정보를 반환합니다.
```

Returns:
```
name, town, townRanks, nationRanks, lastOnline, registered, title, surname, joinedTownAt, friends, uuid
```

### https://planetearth.kr/api/town

Available parameters:
```
uuid=TOWN_UUID : 마을 UUID를 입력하면 해당 마을의 정보를 반환합니다.
name=TOWN_NAME : 마을 이름을 입력하면 해당 마을의 정보를 반환합니다.
```

Returns:
```
name, memberCount, mayor, nation, residents, townBoard, trustedResidents, outlaws, registered, joinedNationAt, founder, spawn, claimSize, uuid
```

### https://planetearth.kr/api/nation

Available parameters:
```
uuid=NATION_UUID : 국가 UUID를 입력하면 해당 마을의 정보를 반환합니다.
name=NATION_NAME : 국가 이름을 입력하면 해당 국가의 정보를 반환합니다.
```

Returns:
```
name, memberCount, capital, leader, towns, allies, enemies, registered, nationBoard, nationSpawn, uuid
```
