# GameFramework-sample

在Assets目录下执行

```
git clone git@github.com:pfcstyle/UnityGameFramework.git
```


在刚刚克隆的UnityGameFramework/Libraries下执行
```
git clone git@github.com:pfcstyle/GameFramework.git
```

删除*UnityGameFramework/Libraries*下的GameFramework.dll

在*UnityGameFramework/Libraries*中创建 GameFramework.asmdef 文件（注意需要勾选unsafe选项）

UnityGameFramework.Runtime.asmdef 依赖 GameFramework.asmdef，取消勾选Use GUIDs, 删除无效的reference

UnityGameFramework.Editor.asmdef 同时依赖 GameFramework.asmdef 和 UnityGameFramework.Runtime.asmdef
