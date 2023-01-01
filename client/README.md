# IL

## GraphQL

- 서버에서 클라이언트가 효율적으로 데이터를 가져오기 위함

## 특장단점

- 하나의 EndPoint 에 여러 API 요청 가능 -> 여러번 API 호출하지 않아도 됨
- 서버의 응답에서 필요한 정보만 요청할 수 있음
- 클라이언트에서만 사용하면 안되고 서버에서도 Apollo 와 같이 작업을 해주어야 사용 가능하다

> 해당 프로젝트에서는 React-Query 와 조합하여 사용하고 있음
> /src/graphql 참고

## meno repo

설정 방법

```
"private": true,
  "workspaces": [
    "client",
    "server"
  ],

 ...
 "scripts": {
    "client": "yarn workspace client dev",
    "server": "yarn workspace server dev",
    "start": "cd server && npm run serve"
  }
```

모노래포란 한 레포 안에 여러가지 프로젝트가 있는 것
또 각 프로젝트의 name 을 변경시킨다 (client, server)
