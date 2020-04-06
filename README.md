# AgoraDynamicKey

Copy from https://github.com/AgoraIO/Tools/tree/master/DynamicKey/AgoraDynamicKey/go , but supply a go module that you can import to your project.

## Usage

```go
import "github.com/bastengao/AgoraDynamicKey/rtctokenbuilder"

expiredAt := uint32(time.Now().Add(time.Hour * 24).Unix())
token, err := rtctokenbuilder.BuildTokenWithUID(appID, appCert, channelName, userID, rtctokenbuilder.RoleSubscriber, expiredAt)
```

More details see [Agora Generate a Token from Your Server](https://docs.agora.io/en/cloud-recording/token_server_go?platform=Go)
